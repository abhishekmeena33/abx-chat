# abx-chat

**First chatbot using PyTorch**

## Overview

abx-chat is a simple chatbot built with PyTorch and Flask. This project integrates a machine learning model trained with PyTorch to understand and respond to basic intents defined in JSON. The chatbot uses a web interface to interact with users.

## Project Structure

- **app.py**: The main Flask application that serves the chatbot and handles API requests.
- **chat.py**: Handles the chatbot logic, including loading the model and processing user input.
- **data.pth**: The trained PyTorch model file.
- **intents.json**: A JSON file containing the training data and intents used to train the chatbot model.
- **model.py**: Defines the neural network architecture for the chatbot.
- **nltk_utils.py**: Contains helper functions using NLTK for text preprocessing.
- **train.py**: A script to train the chatbot model using data from `intents.json`.
- **static**: Contains static assets for the frontend, including CSS and JavaScript.
- **templates**: Contains HTML templates for rendering the chatbot interface.

## Features

- **Machine Learning with PyTorch**: Uses a neural network model to understand and respond to user queries.
- **Flask Integration**: Serves the chatbot via a Flask web application.
- **Interactive Chat Interface**: Allows users to interact with the chatbot through a simple web-based interface.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/abhishekmeena33/abx-chat.git
    ```
2. Navigate to the project directory:
    ```bash
    cd abx-chat
    ```
3. Install the required dependencies

## Usage

1. Run the Flask application:
    ```bash
    python app.py
    ```
2. Open a web browser and go to `http://127.0.0.1:5000` to interact with the chatbot.

## Training the Model

If you want to retrain the model with new intents, you can update `intents.json` and then run:
```bash
python train.py
