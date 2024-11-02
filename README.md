# 🛍️ RAGKart-Advisor: A Flipkart-Inspired Product Recommendation Chatbot

RAGKart-Advisor is an advanced chatbot designed to provide smart product recommendations and answer customer queries about a variety of products, using RAG (Retrieval-Augmented Generation) techniques and LangChain. This project brings together product data from Flipkart, a powerful language model, and an intuitive conversational interface.

## ✨ Project Overview

- **Purpose**: To assist users in finding the best products according to their preferences and answer queries based on product reviews and descriptions.
- **Data Source**: Product data from Flipkart, featuring product titles and reviews to generate relevant and helpful responses.
- **Model**: Powered by Llama 3.1 (70B model) for high-quality conversational responses.
- **Backend Framework**: Flask, providing a web-based interface for user interactions.
- **RAG Concept**: Combines Retrieval-Augmented Generation for generating answers with contextually aware recommendations.
```
## 📂 Project Structure
📦 RAGKART_ADVISOR/
├── 📂 flipkart/
│   ├── __init__.py                     # Package initializer for 'flipkart' module
│   ├── data_converter.py               # Converts and structures data from CSV format
│   ├── data_ingestion.py               # Ingests and processes data into AstraDB
│   ├── retrieval_generation.py         # Builds retrieval and generation chain for RAG
├── 📂 static/
│   └── style.css                       # CSS for styling the HTML frontend
├── 📂 templates/
│   └── index.html                      # Main HTML template for the chatbot interface
├── .env                                # Environment variables for API keys
├── requirements.txt                    # List of required Python packages
├── setup.py                            # Setup configuration for package management
└── app.py                              # Main Flask application file to run the chatbot

```
