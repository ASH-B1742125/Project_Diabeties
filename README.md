# Diabetes Prediction Project

## Team Members
- Arpita Saha
- Devadrita Mitra
- Shilpi Jha
- Ashutosh Bhowmick

## Overview
The Diabetes Prediction Project is a machine learning and web-based application developed using Django. It predicts the likelihood of diabetes in individuals based on medical data attributes using trained machine learning models.

## Scope
- Data-driven analysis of patient health attributes
- Machine learning model integration (scikit-learn)
- Django-based web application with interactive user interface
- Deployment on PythonAnywhere with virtual environment support

## Dataset
The dataset used is `diabetes_prediction_dataset.csv`, containing health-related parameters such as:
- Age
- Gender
- BMI
- Blood Pressure
- Glucose Level
- Insulin
- Other medical indicators

## Requirements
To set up the project locally, install the following:
```bash
pip install -r requirements.txt
```

Main dependencies include:
- Python 3.10
- Django
- scikit-learn
- pandas
- numpy
- matplotlib
- joblib

## Running the Project Locally
1. Clone or download the repository.
2. Navigate to the project directory.
3. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate   # On Linux/Mac
   venv\Scriptsctivate      # On Windows
   ```
4. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```
5. Run database migrations:
   ```bash
   python manage.py migrate
   ```
6. Start the server:
   ```bash
   python manage.py runserver
   ```
7. Open browser at `http://127.0.0.1:8000/`.

## Deployment (PythonAnywhere)
1. Upload project files to PythonAnywhere.
2. Create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate
   pip install -r requirements.txt
   ```
3. Configure WSGI file at `/var/www/username_pythonanywhere_com_wsgi.py`.
4. Update `ALLOWED_HOSTS` in `settings.py` with your PythonAnywhere domain.
5. Collect static files:
   ```bash
   python manage.py collectstatic
   ```
6. Run migrations:
   ```bash
   python manage.py migrate
   ```
7. Reload the web app from the **Web** tab on PythonAnywhere.

## File Structure
```
diabetes_project/
│── diabetes_app/        # Django app
│── staticfiles/         # Static files (CSS, JS, Images)
│── templates/           # HTML templates
│── manage.py
│── requirements.txt
│── Procfile
│── runtime.txt
```

## Results
- The trained ML model predicts whether a patient is likely to have diabetes.
- Model stored using `joblib` and integrated into Django views.
- Front-end interface allows users to enter details and see predictions.

## Future Improvements
- Add more ML algorithms for better accuracy
- Use larger and real-world datasets
- Enhance UI with Tailwind CSS or Bootstrap
- Add user authentication system

## Deployment link

https://ashbow.pythonanywhere.com/
---
✨ Developed with passion by our team for academic submission.
