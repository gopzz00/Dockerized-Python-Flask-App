
# Dockerized Flask App

This is a simple Flask application that displays a welcome message and runs in a Docker container. The project demonstrates how to containerize a basic Python web application using Docker.


## **Features**
- Minimal Flask application
- Dockerized for easy deployment
- Runs on any platform that supports Docker


## **Getting Started**


### **Prerequisites**
- Install [Docker](https://www.docker.com/).


### **Installation and Usage**

1. **Clone the Repository**
   git clone https://github.com/gopzz00/Dockerized-Python-Flask-App.git
   cd dockerized-flask-app

2. **Build the Docker Image**
   docker build -t flask-app .

3. **Run the Docker Container**
   docker run -d -p 5000:5000 flask-app

4. **Access the Application**
   - Open your browser and visit: [http://localhost:5000]



### **Folder Structure**
flask-app/
│
├── app.py              # The main Flask application
├── requirements.txt    # Python dependencies
└── Dockerfile          # Docker configuration



### **Technologies Used**
- **Python**: Programming language used for the Flask app.
- **Flask**: Lightweight web framework for Python.
- **Docker**: To containerize the application.


### **How It Works**
1. The `app.py` script creates a Flask web application with one route (`/`) that returns a welcome message.
2. The `Dockerfile` specifies the setup for a Docker image:
   - Uses the Python 3.9-slim base image.
   - Copies the application files into the container.
   - Installs the required Python dependencies.
   - Runs the Flask application on container start.
3. The app runs on port 5000, which is exposed via Docker.
---
