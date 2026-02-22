# flask-app
# Python Flask Web Application

## 📌 Overview

This project demonstrates the development of a simple Python Flask web application that displays a personalised greeting message in the browser.

The objective of this project was to understand:

- How a Flask application is structured
- How HTTP routing works
- Running a local development server
- Using Git for version control
- Basic cloud deployment considerations

---

## 🛠 Tech Stack

- Python 3
- Flask
- Git
- Linux / WSL environment

---

## 📂 Project Structure
```
.
├── app.py  
├── requirements.txt  
└── README.md  
```
---

## 🧩 Application Code

```python
from flask import Flask

app = Flask(__name__)

@app.route("/")
def hello_world():
    return "<p>Hello Faizal!</p>"

if __name__ == '__main__':
    app.run(host="0.0.0.0", port=8080)
```
---
## ▶ Running the Application Locally

1. Install dependencies:
```
pip install flask
```
2. Run the application:
```
python3 app.py
```
3. Open your browser and visit:
```
http://127.0.0.1:8080
```
---
## 🔁 Git Workflow

The following Git workflow was used:
```
git clone https://github.com/mfaizalbe/flask-app
git add .
git commit -m "Initial Flask application"
git push
```
---
## ☁ Cloud Extension (Next Step)

As an extension, this application can be deployed to an AWS EC2 instance by:

- Launching an Ubuntu or Amazon Linux EC2 instance
- Configuring security group rules (open port 8080)
- Running the Flask app on the instance
- Accessing the application via the EC2 public IP

Future improvements may include:

- Using Gunicorn as a production server
- Adding Nginx as a reverse proxy
- Containerising with Docker
- Deploying via CI/CD pipeline
---

## 📈 Learning Outcome

This project strengthened my understanding of:

- Backend web development fundamentals
- Request–response lifecycle
- Local development environments
- Git-based version control
- Introductory cloud deployment concepts
---

## 🙏 Acknowledgements
[NTU SCTP - Coaching 2: Building a Python Flask Application](https://docs.google.com/document/d/1ZZJ72f_YxlDUN2dejZJu2cfU8JYwn6xKuTY1eGN6Dtw)
