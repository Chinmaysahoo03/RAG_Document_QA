# RAG-Enhanced Document Q&A System

An advanced Retrieval-Augmented Generation (RAG) system for querying and answering questions over large documents or PDFs using semantic search and LLMs. Built with LangChain, Groq, and Hugging Face models for efficient document ingestion, vector-based retrieval, and context-aware responses.

## Features
- **Document Ingestion**: Supports PDF and text files with chunking and cleaning.
- **Semantic Search**: Uses Sentence Transformers for embeddings and FAISS for fast vector retrieval.
- **LLM Integration**: Leverages Groq's Gemma-2-9B-IT for accurate, cited answers.
- **Interactive Q&A**: Handles multi-query sessions with source citations.
- **Deployment**: Runnable in Google Colab; optional Streamlit UI for demos.

## Tech Stack
- **Languages/Frameworks**: Python, LangChain, Groq API.
- **Embeddings & Retrieval**: Hugging Face Sentence Transformers, FAISS.
- **Document Processing**: PyPDFLoader, RecursiveCharacterTextSplitter.
- **Requirements**: Groq API key (free tier), GPU optional for embeddings.

## Installation
1. Clone the repo:

2. In Google Colab (recommended):
- Open a new notebook and copy the provided cells.
- Install dependencies: `!pip install langchain-groq langchain sentence-transformers faiss-cpu pypdf streamlit`
3. Set Groq API Key: In Colab Secrets (Sidebar > Secrets), add `GROQ_API_KEY` from [console.groq.com](https://console.groq.com).

## Usage
1. **Upload Document**: Run Cell 3 to upload a PDF (e.g., research paper).
2. **Build Index**: Execute Cells 4-5 to process and index the document.
3. **Query**: In Cell 6, ask questions like "What is the main topic?" – get answers with sources.
4. **Streamlit Demo** (Optional): Copy Cell 7 to `app.py` and run `!streamlit run app.py` for a web UI.

Example Output:

## Code Structure
- **Cell 1-2**: Dependencies and setup (embeddings, LLM).
- **Cell 3**: Load and split documents.
- **Cell 4**: Build FAISS vector store.
- **Cell 5**: RAG chain configuration.
- **Cell 6**: Interactive Q&A loop.
- **Cell 7**: Streamlit snippet.

## Contributing
Fork the repo, add features (e.g., multi-document support), and submit a PR. Ensure compatibility with free tools.

## License
MIT License – feel free to use and modify.

## Contact
Chinmaya Sahoo – chinmayasahoo3210@gmail.com  
Built with ❤️ for Gen AI exploration.
