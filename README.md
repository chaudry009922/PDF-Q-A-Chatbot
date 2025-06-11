# PDF Q&A Chatbot 

This project is an interactive PDF Question-Answering chatbot powered by OpenAI's LLMs, LangChain, and Gradio. Users can upload any PDF document and ask natural language questions based on its content.

## Features

- Upload any PDF file
- Extracts and indexes PDF content
- Asks questions in plain English
- Uses OpenAI API for answering
- Gradio-based web UI in the same notebook

## Tech Stack

- Python
- OpenAI GPT (via LangChain)
- FAISS (for vector storage)
- PyPDF2 (for PDF reading)
- Gradio (UI interface)

## Setup Instructions

### 1. Clone or open the Colab notebook

Or use your own environment with the instructions below.

### 2. Add your own api key 
os.environ["OPENAI_API_KEY"] = "your-openai-api-key-here"
You can get your API key from https://platform.openai.com/account/api-keys

### 4. Run the Notebook
Run the main cell 

Text is split into chunks and converted to embeddings using OpenAI

FAISS stores the embeddings for fast retrieval

LangChain’s RetrievalQA uses a retriever + LLM for answers

Gradio lets users upload and ask questions in a web UI

Example Questions
"What is the main topic of this document?"

"Summarize the third page."

"What are the key findings?"

Author
Usama Ashraf
Machine Learning Enthusiast from Pakistan

Made with dedication and hard work.

```bash
pip install -r requirements.txt



