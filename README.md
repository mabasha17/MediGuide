# Medicine Recommendation System

A Flask-based web application that uses machine learning to predict diseases based on symptoms and provide comprehensive health recommendations.

## Features

- **Disease Prediction**: AI-powered symptom analysis to predict 41 different diseases
- **Comprehensive Recommendations**: Get detailed information including:
  - Disease descriptions
  - Precautions
  - Medications
  - Diet recommendations
  - Workout/lifestyle suggestions
- **Modern UI**: Responsive Bootstrap-based interface
- **Real-time Results**: Instant predictions and recommendations

## Supported Diseases

The system can predict and provide recommendations for 41 diseases including:

- Fungal infection, Allergy, GERD
- Diabetes, Hypertension, Migraine
- Various types of Hepatitis (A-E)
- Tuberculosis, Pneumonia, Typhoid
- Heart attack, Arthritis, and more

## Technology Stack

- **Backend**: Python Flask
- **Machine Learning**: Scikit-learn (SVC, Random Forest)
- **Frontend**: HTML, CSS, Bootstrap 5
- **Data Processing**: Pandas, NumPy
- **Model Storage**: Pickle files

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Medicine-Recommendation-System.git
cd Medicine-Recommendation-System
```

2. Create a virtual environment:

```bash
python -m venv venv
```

3. Activate the virtual environment:

```bash
# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

4. Install required packages:

```bash
pip install flask pandas numpy scikit-learn
```

## Usage

1. Start the Flask application:

```bash
python main.py
```

2. Open your web browser and navigate to:

```
http://localhost:5000
```

3. Enter your symptoms separated by commas (e.g., "cough, fever, headache")

4. Get instant disease prediction and comprehensive recommendations

## Project Structure

```
Medicine-Recommendation-System/
├── main.py                          # Flask application
├── templates/                       # HTML templates
│   ├── index.html                   # Main application page
│   ├── about.html                   # About page
│   ├── contact.html                 # Contact page
│
├── static/                         # Static assets
│   └── heal.jpg                    # Application image
├── dataset/                        # Dataset files (not included in this repo)
├── model/                          # Trained ML models (not included in this repo)
└── README.md                       # This file
```

## API Endpoints

- `GET /` - Home page with symptom input form
- `POST /predict` - Disease prediction endpoint
- `GET /about` - About page
- `GET /contact` - Contact page

## Machine Learning Model

- **Primary Model**: Support Vector Classifier (SVC) with linear kernel
- **Accuracy**: 100% on test data
- **Features**: 132 symptoms mapped to binary vectors
- **Output**: 41 different disease predictions
