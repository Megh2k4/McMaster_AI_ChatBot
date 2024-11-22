# McMaster_AI_ChatBot

## Overview

This project is a conversational AI chatbot designed to interact with users in a natural and engaging manner. The chatbot leverages machine learning techniques to understand user inputs and provide appropriate responses, simulating a human-like conversation experience.

## Features

- **Natural Language Understanding**: Utilizes a neural network to interpret and classify user inputs.
- **Responsive Conversation**: Provides relevant responses based on predefined intents and patterns.
- **Data Scraping**: Employs Scrapy to gather data for training and expanding the chatbot's knowledge base.
- **Web Interface**: Interactive frontend built with HTML, CSS, and JavaScript for seamless user interaction.

## Tech Stack

- **Frontend**:
  - **HTML5**
  - **CSS3**
  - **JavaScript**

- **Backend**:
  - **Python**
  - **PyTorch** (for building and training the neural network)
  - **Scrapy** (for data scraping)

## Getting Started

### Prerequisites

- Python 3.x
- PyTorch
- Scrapy
- NLTK (Natural Language Toolkit)
- Web browser (for frontend interaction)

### Installation

1. **Clone the Repository**

   ``git clone https://github.com/Megh2k4/McMaster_AI_ChatBot.git``
   
   ``cd McMaster_AI_ChatBot``

3. **Install Dependencies**

    ``import nltk``
   
    ``nltk.download('punkt') ``

5. **Run the app**

    ``python app.py``

## How It Works

## Text Processing

Tokenization: The input sentence is broken down into individual words.
Bag-of-Words Model: Converts the tokenized sentence into a numerical format that the model can understand.

## Neural Network
- Built using PyTorch.
- Input Layer: Receives the bag-of-words vector.
-  Hidden Layers: Two layers with ReLU activation and Dropout for regularization.
- Output Layer: Outputs probabilities for each intent using Softmax.

## Inference
- The model predicts the intent of the user's input.
- Based on the predicted intent and a confidence threshold, an appropriate response is selected.
- If the confidence is low, a default fallback response is provided.

## AI and Machine Learning Details
- Natural Language Processing (NLP): Utilizes NLTK for text preprocessing tasks like tokenization.
- Machine Learning Model: A feedforward neural network trained to classify user inputs into predefined intents.
- Training:
  - The model is trained on the dataset defined in intents.json.
  - Uses Cross-Entropy Loss and the Adam optimizer.
- Activation Functions:
  - ReLU: Introduces non-linearity, allowing the model to learn complex patterns.
  - Softmax: Converts output scores into probabilities for intent classification.
- Regularization:
  - Dropout Layers: Prevents overfitting by randomly deactivating neurons during training.
