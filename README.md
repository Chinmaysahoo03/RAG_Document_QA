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

RAG Q&A System Ready! Type 'quit' to exit.

Question: give an overview of the pdf

Answer: This document outlines a plan for developing an Android app focused on tenant search and PG (Paying Guest) management. 

**Key Features:**

* **Tenant Search:**  Users can search for suitable PG accommodations.
* **PG Details:**  Comprehensive information about available PGs.
* **Booking:**  A streamlined booking process for tenants.
* **Admin Features:** Basic administrative functionalities for managing the platform.

**Development Process:**

* **Sprint-Based:** The project is structured into sprints with specific tasks and deadlines.
* **Tools:**  Android Studio, Figma, Firebase, GitHub, and Postman are utilized for coding, design, backend integration, version control, and API testing.
* **AI Assistance:** GitHub Copilot is employed for code suggestions and debugging.
* **Testing:** JUnit is used for unit testing, and Firebase App Distribution handles test APK distribution.

**Deliverables:**

* **Android APK:** A functional app with all the aforementioned features.
* **GitHub Repository:**  Source code, well-documented, in a private repository.
* **Demo Video:** A short video showcasing the app's functionality.
* **Documentation:**  A guide on running the app and using Firebase.
* **Optional Figma Prototype:**  Interactive prototypes of key screens (if time permits).

**Previous Work:**

The developer highlights two previous projects: a movie streaming app and an urban service app, both built with Jetpack Compose and Kotlin.


Let me know if you have any other questions.


Sources:
[Chunk 1]: – Fix UI bugs and ensure the app looks good on all devices.
– Task: Wrapping up admin features and testing.
• Day 13-14: Final Touches
– Create a demo APK and record a short video showing the app.
– W... (Page: N/A)
[Chunk 2]: After the sprint, Ill deliver:
• Android APK: A working app with tenant search, PG details, booking, and basic owner/admin
features.
• GitHub Repo : All code, documented, in a private repo.
• Demo Vid... (Page: N/A)
[Chunk 3]: 8.1 AI Usage
• Code Help : GitHub Copilot to suggest small code snippets (e.g., ViewModel boilerplate).
• Debugging: Copilot to spot errors like missing null checks.
• Manual Work: Ill write UI code, ... (Page: N/A)

Question: quit

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
