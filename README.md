# Question-Answering Model from PDF Documents

## Overview
This project demonstrates the development of a sophisticated Question-Answering (QA) model capable of retrieving and answering queries from PDF documents with high accuracy. The model uses advanced embedding and retrieval techniques to ensure precise and contextually relevant answers.

## Features
High Accuracy: Achieves 90% accuracy in answering questions based on content from PDF documents.
Advanced Embeddings: Utilizes Hugging Face's BGE model, sentence_transformers, and torch for effective document embeddings.
Efficient Retrieval: Implements RAG (Retrieval-Augmented Generation) and LangChain for enhanced question retrieval and response generation.
Scalable Vector Database: Integrates Qdrant vector database for fast and scalable search operations.
PDF Parsing: Uses pypdf for extracting text from PDFs to facilitate question answering.

# Technologies Used
- Languages & Libraries: Python, Hugging Face's BGE model, sentence_transformers, torch, pypdf
- Database: Qdrant vector database
- Containerization: Docker
- Embedding Techniques: Embedding models and sentence_transformers

## Getting Started
Prerequisites
- Python 3.7 or higher
- Docker
- Required Python libraries (listed in requirements.txt)

## Command to Run
```
docker info
docker pull qdrant/qdrant 
docker run -p 6333:6333 -v .:/qdrant/storage qdrant/qdrant
```

## Then open the terminal in pwd:
```
python -m venv .venv 
cd .venv 
cd scripts 
./activate
cd ..
cd ..
pip install -r requirements.txt
```

- run the ingest.py to create the embeddings. Once the embeddings are created,
- run the app.py to retrieve the relevant docs/chunks

## Result
![image](https://github.com/user-attachments/assets/1fec6763-1783-4074-847a-1d04fb90a62b)


