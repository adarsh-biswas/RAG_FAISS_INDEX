# Chat with PDF using AWS Bedrock (Llama 3 + Titan Embeddings)

This is a GUI-based Retrieval-Augmented Generation (RAG) application built with Python and Tkinter. It allows users to:

- Upload and index PDF documents.
- Create or update a FAISS vector store.
- Query the documents using natural language.
- Get intelligent answers using Meta's LLaMA 3 model served via AWS Bedrock.

---

## Features

- PDF ingestion and chunking using LangChain tools  
- Embedding with **Amazon Titan Text Embeddings v2**  
- Storage and retrieval with **FAISS**  
- Question answering via **Meta LLaMA 3** (8B instruct) on AWS Bedrock  
- Simple Tkinter GUI interface  

---

## About AWS Bedrock and AI Models Used

### What is AWS Bedrock?

**Amazon Bedrock** is a fully managed service that provides access to foundation models (FMs) from multiple leading AI companies via a unified API, without managing infrastructure. You can integrate models from Amazon, Meta, Anthropic, Cohere, and others directly into your apps.

This app uses two key models from AWS Bedrock:

### 1. Amazon Titan Embeddings v2 (`amazon.titan-embed-text-v2:0`)

- A model that converts text into dense vector representations (embeddings).
- Used to transform chunks of PDF content into numerical form.
- These embeddings are stored and later retrieved using FAISS for similarity search.

### 2. Meta LLaMA 3 (8B Instruct) (`meta.llama3-8b-instruct-v1:0`)

- A state-of-the-art large language model designed for instruction-following tasks.
- Used to generate detailed answers based on retrieved document chunks and user queries.
- Capable of generating responses with reasoning and summarization over long contexts.

---

## Requirements

Install the following Python packages:

```
pip install boto3 langchain langchain-community langchain-aws faiss-cpu tkinter
```
