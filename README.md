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

## 🚀 Features

- **Product Recommendation**: Recommends products based on customer descriptions and budget constraints.
- **Query Context Awareness**: Tracks conversation history, improving response accuracy by remembering prior questions.
- **Efficient Data Handling**: Uses AstraDB as a vector store for efficient document retrieval.

## 🔧 Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/datascientistabhishek/RAGKart-Advisor-.git
    cd RAGKart-Advisor
    ```

2. **Set Up the Environment**:
    Create a virtual environment and install dependencies.
    ```bash
    python -m venv ragenv
    source ragenv/bin/activate  # For Linux/MacOS
    .\ragenv\Scripts\activate   # For Windows
    pip install -r requirements.txt
    ```

3. **Set Environment Variables**:
    Create a `.env` file with the following keys:
    ```
    GROQ_API_KEY=your_groq_api_key
    ASTRA_DB_API_ENDPOINT=your_astra_db_api_endpoint
    ASTRA_DB_APPLICATION_TOKEN=your_astra_db_application_token
    ASTRA_DB_KEYSPACE=your_keyspace
    HF_TOKEN=your_huggingface_token
    ```

4. **Ingest Data**:
    Run `data_ingestion.py` to load the product data into AstraDB.
    ```bash
    python -m flipkart.data_ingestion
    ```

5. **Launch the Application**:
    Start the Flask app.
    ```bash
    python app.py
    ```

    Access the chatbot at `http://127.0.0.1:5000`.

## 🛠️ Usage

1. **Interact with the Chatbot**:
    - Go to the web interface and type in a product-related query.
    - For example, "Can you recommend a budget-friendly smartphone?"

2. **Chat History**:
    - The chatbot retains context to improve multi-turn conversations.

## 💼 Technologies Used

- **Language Model**: Llama 3.1 (70B model) by Groq
- **Vector Store**: AstraDBVectorStore (AstraDB for storage and retrieval)
- **Frameworks**: LangChain for RAG, Flask for backend
- **Languages**: Python, HTML, CSS (for styling)
- **Other Tools**: dotenv for environment management


## 🤝 Contributions

Contributions, issues, and feature requests are welcome. Feel free to check the issues page if you want to contribute.

---

**Developed by** Abhishek Singh

