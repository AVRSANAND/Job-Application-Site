# Job Application Site

This project is a simple job application web app built using Flask. The app allows users to submit their details such as name, email, availability, and occupation, and sends a confirmation email to the user upon successful submission.

## Features

- User can submit job application details through a form.
- Form data is stored in a SQLite database.
- Confirmation email is sent to the user after form submission.
- Flash messages are used to display form submission success.

## Technologies Used

- **Flask**: Web framework used to build the application.
- **Flask SQLAlchemy**: ORM used to interact with the SQLite database.
- **Flask-Mail**: Used for sending email notifications.
- **HTML/CSS**: Frontend structure using Bootstrap 5 for styling.

## Installation

1. Clone the repository:

```bash
git clone https://github.com/AVRSANAND/Job-Application-Site
cd Job-Application-Site
```

2. Create a SQLite database:
```bash
python
>>> from app import db
>>> db.create_all()
>>> exit()
```

3. Update email settings in app.py with your own credentials:
```python
app.config["MAIL_USERNAME"] = "your-email@gmail.com"
app.config["MAIL_PASSWORD"] = "your-password"
```

## Usage
1. Run the Flask application:
```bash
python app.py
```
2. Open your browser and go to http://127.0.0.1:5001/.
3. Fill out the form with your details and submit.
4. Upon submission, a confirmation email will be sent to the email address provided.
