# Chatbot using NLP and Streamlit

## Introduction
This project implements a chatbot using Natural Language Processing (NLP) techniques and Logistic Regression for intent classification. The chatbot is designed to understand user queries and respond based on predefined intents. The interface is built using Streamlit, a Python library for creating interactive web applications.

## Features
- **Natural Language Processing (NLP)**: Uses the TF-IDF vectorizer to convert text into numerical form.
- **Machine Learning Model**: Logistic Regression is used to classify user inputs based on intents.
- **Streamlit Interface**: Provides a simple web-based interface for user interaction.
- **Chat Logging**: Stores conversation history in a CSV file for reference.
- **Predefined Intents**: Uses a JSON file containing patterns and responses to generate replies.

## Technologies Used
- Python
- Natural Language Toolkit (NLTK)
- Scikit-learn
- Streamlit
- JSON
- CSV

## Installation
Ensure you have Python installed on your system. Then, install the required dependencies using:
```bash
pip install streamlit scikit-learn nltk
```

## Setup
1. Download or clone the repository.
2. Place the `intents.json` file in the same directory as the script.
3. Ensure `nltk_data` is available or downloaded in the project directory.
4. Run the chatbot using:
   ```bash
   streamlit run chatbot.py
   ```

## How It Works
1. **Load Intents**: Reads the `intents.json` file containing predefined user intents and responses.
2. **Train Model**: Uses TF-IDF vectorization on input patterns and trains a Logistic Regression model.
3. **User Interaction**:
   - The user inputs a message.
   - The input is transformed and classified into an intent.
   - A response is selected randomly from the corresponding intent responses.
4. **Chat Logging**: Saves conversations in `chat_log.csv` for future reference.

## Usage
- Start the chatbot interface using Streamlit.
- Type messages in the input field and receive chatbot responses.
- View past conversations under the "Conversation History" tab.

## Future Improvements
- Incorporate deep learning models (e.g., LSTMs, Transformers) for better intent recognition.
- Expand the intents dataset for improved chatbot capabilities.
- Enhance the UI with better design and real-time interaction features.

## Author
Sanket G Shanbhag

