# 📚 Statistics RAG Assistant

An AI-powered PDF Question Answering System built using Python, Streamlit, LangChain, NVIDIA AI, FastEmbed, and Qdrant.

The application allows users to ask questions related to Statistical Techniques and receive AI-generated answers based on information retrieved from PDF documents.

## 🚀 Project Overview

The Statistics RAG Assistant uses **Retrieval-Augmented Generation (RAG)** to provide accurate, context-based answers from statistical study materials.

Instead of generating answers only from general AI knowledge, the system retrieves relevant information from PDF documents and uses NVIDIA AI to generate responses based on the retrieved context.

## ✨ Key Features

- 📄 PDF document support.
- 📤 PDF upload interface using Streamlit.
- 🤖 AI-powered question answering.
- 🔍 Intelligent document retrieval.
- 🧠 Text embeddings using FastEmbed.
- 🗄️ Vector storage using Qdrant.
- ⚡ NVIDIA Nemotron LLM integration.
- 📖 Context-based answers from statistical study materials.
- 🐍 Python-based backend.
- 💻 Interactive web interface.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | Web application interface |
| LangChain | RAG pipeline development |
| NVIDIA AI | Large Language Model |
| Nemotron | AI response generation |
| FastEmbed | Text embeddings |
| Qdrant | Vector database |
| PyPDFLoader | PDF text extraction |
| RecursiveCharacterTextSplitter | Text chunking |
| python-dotenv | Environment variable management |

## 🏗️ System Architecture

The application follows a Retrieval-Augmented Generation architecture.

```text
          User
           |
           v
    Streamlit Interface
           |
           v
       PDF Document
           |
           v
      PDF Extraction
           |
           v
       Text Splitting
           |
           v
    FastEmbed Embeddings
           |
           v
     Qdrant Vector Store
           |
           v
     Similarity Search
           |
           v
     Relevant Context
           |
           v
      NVIDIA Nemotron
           |
           v
      Generated Answer
           |
           v
    Display Answer to User
```

## 📂 Project Structure

```text
Statistics-RAG-Assistant/
│
├── .venv/
│
├── __pycache__/
│
├── .env
│
├── .gitignore
│
├── main.py
│
├── requirement.txt
│
└── STATS.pdf
```

**File Description:**

- `main.py` – Main Python application containing the Streamlit interface and RAG functionality.
- `requirement.txt` – Contains the required Python dependencies.
- `STATS.pdf` – Statistical Techniques study material.
- `.env` – Stores the NVIDIA API key.
- `.gitignore` – Prevents sensitive and unnecessary files from being uploaded to GitHub.
- `.venv/` – Python virtual environment.

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_LINK
```

### 2. Navigate to the Project Directory

```bash
cd Statistics-RAG-Assistant
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

### 4. Activate Virtual Environment

For Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 5. Install Dependencies

```bash
pip install -r requirement.txt
```

### 6. Configure Environment Variables

Create a `.env` file in the project root directory.

Add your NVIDIA API key:

```env
NVIDIA_API_KEY=your_nvidia_api_key
```

Get your API key from:

https://build.nvidia.com/

**Important:** Never upload your actual `.env` file or API key to GitHub.

### 7. Run the Application

```bash
streamlit run main.py
```

### 8. Open in Browser

Visit:

```text
http://localhost:8501
```

Your Statistics RAG Assistant should now be accessible through your browser.

## 💡 How It Works

**Step 1: PDF Loading**

The application loads statistical study material from a PDF document.

**Step 2: Text Extraction**

PyPDFLoader extracts readable text from the PDF.

**Step 3: Text Chunking**

RecursiveCharacterTextSplitter divides extracted text into smaller chunks for efficient retrieval.

**Step 4: Embedding Generation**

FastEmbed converts text chunks into numerical vector representations.

**Step 5: Vector Database**

Qdrant stores the generated embeddings for similarity searching.

**Step 6: Question Processing**

The user enters a question through the Streamlit interface.

**Step 7: Information Retrieval**

The system retrieves the most relevant text chunks from the vector database.

**Step 8: AI Response Generation**

NVIDIA Nemotron uses the retrieved context to generate an answer.

**Step 9: Display Result**

The generated answer is displayed to the user through the application interface.

## 🧪 Example Questions

Users can ask questions such as:

1. What are the methods of data collection?
2. Explain correlation and regression.
3. What is the principle of least squares?
4. Explain measures of central tendency.
5. What is standard deviation?
6. Explain probability distributions.

Answers depend on the information available in the uploaded or configured PDF document.

## 🔐 Security

- API keys are stored in environment variables.
- `.env` is excluded from GitHub.
- Virtual environment files are excluded from version control.
- Sensitive credentials should never be committed to the repository.

## 🎯 Project Objectives

- Develop an AI-powered PDF question-answering application.
- Apply Retrieval-Augmented Generation techniques.
- Simplify access to statistical study materials.
- Integrate vector embeddings and semantic search.
- Generate context-based answers using NVIDIA AI.
- Build an interactive interface using Streamlit.

## 🔮 Future Enhancements

- Support multiple PDF documents.
- Improve PDF upload and document indexing.
- Add chat history.
- Display PDF page references with answers.
- Improve document retrieval accuracy.
- Add support for additional academic subjects.
- Deploy the application online.

## 👨‍💻 Author

**Nageshranjan265**

GitHub: https://github.com/nageshranjan265-oss

## 📜 License

This project is developed for educational and learning purposes.
