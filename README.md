# 🧠 RAG Document Q&A with Groq, LLaMA3 & OpenAI Embeddings
An advanced Retrieval-Augmented Generation (RAG) application that allows users to interact with research papers using natural language queries. Built with Langchain, this Streamlit-powered interface uses OpenAI Embeddings to transform PDF content into a searchable vector database and Groq’s LLaMA3 model for lightning-fast responses.

## 📌 Features
* 🔍 Ask questions directly from your research papers (PDFs)
* ⚡ Powered by Groq's ultra-fast inference of LLaMA3
* 🧠 Intelligent search with OpenAI Embeddings + FAISS
* 📄 Multi-document PDF ingestion and chunking
* 🖥️ Simple, elegant interface via Streamlit
* 🧰 Modular RAG pipeline using Langchain components

## 🧠 Technologies Used
* Langchain
* Streamlit
* Groq API (LLaMA3-8B-8192)
* OpenAI Embeddings
* FAISS (Vector Store)
* Python-dotenv
* PyPDFDirectoryLoader
* RecursiveCharacterTextSplitter

## 🗂 Project Structure
```
├── app.py                    # Main Streamlit application
├── research_papers/         # Folder for uploading your PDF research papers
├── requirements.txt         # Python dependencies
└── .env                     # Your API keys (do NOT share this file)
```

## ⚙️ Setup Instructions
1. Clone the Repository
```
git clone https://github.com/bhaskar2311/RAG-Document-QnA-Groq-Llama3-OpenAIEmbeddings
cd RAG-Document-QnA-Groq-Llama3-OpenAIEmbeddings
```
2. Create a Virtual Environment (optional but recommended)
```
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
3. Install Dependencies
```
pip install -r requirements.txt
```
4. Setup Environment Variables
  * Create a .env file in the root directory and add your API keys like this:
```
# .env
OPENAI_API_KEY=your_openai_api_key_here
LANGSMITH_API_KEY=your_langsmith_key_here
```
🚨 Warning: Never commit .env files to public repositories.

## 🚀 How to Run
#### 🧠 Using OpenAI (app.py)
```
streamlit run app.py
```
* Upload your PDF files to the research_papers/ folder.
* Click Document Embedding to create the vector store.
* Ask a question related to the PDF content.
* View the concise answer and supporting context via the Document Similarity Search.

## 📦 Reusability
* This application is designed to be easily extended:

  - Swap in another embedding model (e.g., HuggingFace)

  - Replace Groq with OpenAI or Ollama models

  - Ingest multiple document types beyond PDFs

 ## 📸 Screenshots
 ![Output ](https://github.com/user-attachments/assets/764970bd-f86d-44cc-a739-ea8229b328e8)
 ![Output with Document Similarity Search](https://github.com/user-attachments/assets/9da8c72a-9a3c-4099-a09a-54814e93299b)

 ## 📝 Notes
This project was fully developed by me. The README was written based on my knowledge and experience, with support from generative AI tools to refine its structure and presentation.

## 📄 License
This project is open source and available under the MIT License.

## 🙋‍♂️ Author
Made with ❤️ by Bhaskar Shivaji Kumbhar





