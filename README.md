# AI Chatbot Using NLP, Scikit-Learn, and Flask

## Project Overview

This project implements an AI-powered chatbot using Natural Language Processing (NLP). The chatbot identifies user intents from text input and generates appropriate responses. It is built using Python, Scikit-Learn, NLTK, and Flask.

The system uses an intent dataset in JSON format, trains a machine learning model for intent classification, and serves responses through a Flask-based web application.

---

## Objectives

* Understand intent classification in conversational AI.
* Build a chatbot using NLP techniques.
* Train a machine learning model for intent prediction.
* Deploy the chatbot through a Flask API.
* Create a simple web-based chatbot interface.

---

## Technologies Used

* Python
* NLTK (Natural Language Toolkit)
* Scikit-Learn
* Flask
* HTML
* JSON
* Pickle

---

## Project Structure

Chatbot_Project/

├── intents.json

├── train.py

├── chatbot.py

├── app.py

├── model.pkl

├── vectorizer.pkl

├── templates/

│   └── index.html

├── static/

├── README.md

└── screenshots/

---

## Dataset Description

The chatbot uses a custom intent dataset stored in `intents.json`.

Each intent contains:

* Tag (Intent Name)
* Sample User Queries (Patterns)
* Bot Responses

Example:

```json
{
  "tag": "greeting",
  "patterns": ["Hi", "Hello", "Hey"],
  "responses": ["Hello!", "Hi there!", "Welcome!"]
}
```

---

## Features

* Intent Classification
* Text Vectorization using TF-IDF
* Machine Learning Model using Logistic Regression
* Rule-Based Response Selection
* Flask REST API
* Web-Based Chat Interface
* Easy to Extend with New Intents

---

## Implementation Workflow

### Step 1: Create Intent Dataset

Create a JSON file containing intents, patterns, and responses.

### Step 2: Train the Model

The training script:

* Loads intents from JSON.
* Converts text into numerical vectors using TF-IDF.
* Trains a Logistic Regression classifier.
* Saves the trained model and vectorizer.

### Step 3: Build Chatbot Logic

The chatbot:

* Accepts user input.
* Converts text using the saved vectorizer.
* Predicts intent using the trained model.
* Returns a suitable response.

### Step 4: Create Flask API

The Flask server:

* Hosts the chatbot.
* Accepts user messages.
* Sends responses back to the client.

### Step 5: Create Web Interface

A simple HTML page allows users to interact with the chatbot through a browser.

---

## Installation

Install required libraries:

```bash
pip install nltk
pip install scikit-learn
pip install flask
pip install pandas
pip install numpy
```

Download NLTK resources:

```python
import nltk

nltk.download('punkt')
nltk.download('wordnet')
nltk.download('omw-1.4')
```

---

## How to Run the Project

### Train the Model

```bash
python train.py
```

Output:

```text
Training Completed
```

Generated Files:

```text
model.pkl
vectorizer.pkl
```

### Run Flask Server

```bash
python app.py
```

Output:

```text
Running on http://127.0.0.1:5000
```

### Open Browser

```text
http://127.0.0.1:5000
```

---

## Example Conversation

User: Hello

Bot: Hi there!

User: What is this chatbot?

Bot: I am an AI chatbot built using Python and NLP.

User: Thanks

Bot: You're Welcome

User: Bye

Bot: Goodbye!

---

## Evaluation Metrics

The chatbot performance can be evaluated using:

* Accuracy Score
* Classification Report
* Intent Prediction Results

Example:

```python
from sklearn.metrics import accuracy_score
```

---

## Learning Outcomes

After completing this project, the following concepts are learned:

* Natural Language Processing
* Intent Classification
* Text Vectorization
* Machine Learning Model Training
* Flask API Development
* Web Application Deployment
* Chatbot Design Principles

---

## Deliverables

* Source Code
* Intent Dataset (JSON)
* Training Script
* Flask API Server
* Trained Model
* Chatbot Interface
* README Documentation
* Screenshots
* Demo Video
* GitHub Repository Link

---

## Future Enhancements

* Add more intents and responses.
* Integrate deep learning models.
* Add database support.
* Implement user authentication.
* Add voice-based interaction.
* Connect with external APIs.

---

## Screenshots

Add the following screenshots:

1. Project Folder Structure
2. Training Output
3. Chatbot Testing
4. Flask Server Running
5. Browser Interface
6. Accuracy Results
7. GitHub Repository

---

## Conclusion

This project successfully demonstrates the development of an AI chatbot using NLP techniques, Scikit-Learn for intent classification, and Flask for deployment. The chatbot can understand user intents and provide meaningful responses through a web-based interface.
