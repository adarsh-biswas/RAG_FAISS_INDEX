# 📄 Chat with PDF using AWS Bedrock (Llama 3 + Titan Embeddings)

This is a GUI-based Retrieval-Augmented Generation (RAG) application built with Python and Tkinter. It allows users to:

- Upload and index PDF documents.
- Create or update a FAISS vector store.
- Query the documents using natural language.
- Get intelligent answers using Meta's LLaMA 3 model served via AWS Bedrock.

---

## 🚀 Features

- PDF ingestion and chunking using LangChain tools  
- Embedding with **Amazon Titan Text Embeddings v2**  
- Storage and retrieval with **FAISS**  
- Question answering via **Meta LLaMA 3** (8B instruct) on AWS Bedrock  
- Simple Tkinter GUI interface  

---

## 🧰 Requirements

Install the following Python packages:

```
pip install boto3 langchain langchain-community langchain-aws faiss-cpu tkinter
```
