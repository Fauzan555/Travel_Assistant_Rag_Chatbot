# Toronto Travel Assistant - RAG Chatbot

This project is a **Retrieval-Augmented Generation (RAG) chatbot** that assists users with travel information about Toronto.  
It combines **document processing, embeddings, vector storage, and large language models** to provide concise, context-aware answers.

The repository contains two main components:  

1. `RAG_ChatBot.py` - Backend that handles document processing, vector embeddings, and LLM responses.  
2. `streamlitMain.py` - Streamlit frontend for interactive chat.

---

## Features

- Loads and splits large documents into manageable chunks for better retrieval.  
- Generates embeddings using HuggingFace models.  
- Stores vectors in Pinecone for fast semantic search.  
- Uses a structured prompt template tailored for Toronto travel queries.  
- Interactive chat interface via Streamlit.  
- Concise answers limited to two sentences per response.  

---

## Tech Stack

- Python 3.10+  
- [LangChain](https://www.langchain.com/) for RAG workflows  
- [Pinecone](https://www.pinecone.io/) as vector database  
- [OpenAI GPT-3.5 / ChatOpenAI](https://platform.openai.com/) for generating responses  
- HuggingFace embeddings (`sentence-transformers`)  
- `dotenv` for environment variables  
- Streamlit for frontend chat interface  

---

## Detailed Project Steps

### 1. Loading and Splitting Documents
We load the knowledge base from a `.txt` file containing Toronto travel information:

# Project Structure
.
├── materials/
│   └── torontoTravelAssistant.txt    # Knowledge base
├── RAG_ChatBot.py                    # Chatbot backend
├── streamlitMain.py                  # Streamlit frontend
├── .env                              # Environment variables
├── requirements.txt                  # Python dependencies
└── README.md                         # Project documentation

# Installation
git clone https://github.com/your-username/toronto-travel-assistant.git
cd toronto-travel-assistant
