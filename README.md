# RAG-System

An advanced Retrieval-Augmented Generation (RAG) system built with LangChain, capable of processing PDF and PPT files to provide educational explanations on any topic.

## Features

- **Document Processing**: Support for PDF and PPT files
- **Advanced Text Chunking**: Recursive character text splitting with overlap
- **State-of-the-Art Embeddings**: Using Ollama embeddings
- **Hybrid Retrieval**:
  - Dense retrieval with FAISS
  - Sparse retrieval with BM25
  - Cohere Reranker for result optimization
- **Streaming Responses**: Real-time response generation
- **Conversation History**: Maintains context across multiple queries
- **Performance Logging**: Tracks processing time for optimization

## Prerequisites

- Python 3.8+
- Ollama installed and running locally
- Cohere API key

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd rag-system
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```


## Usage

1. Start Ollama server locally

2. Run this command
   ```
   python app.py
   ```

## Performance Considerations

- Document processing time depends on file size and complexity
- Initial retriever setup requires embedding generation for all chunks
- Query response time varies based on:
  - Document corpus size
  - Query complexity
  - Number of retrieved documents
  - Reranking process
  - 
## Closed Source

This project is not open source and its code is not publicly available.
