# RAG Application using Gemini Pro

This is a **Retrieval-Augmented Generation (RAG)** application built with **Streamlit** and **LangChain**.  
It allows users to upload a PDF document and query it using **Google's Gemini Pro** model with vector search powered by **ChromaDB**.

---

## 🚀 Features
- PDF ingestion using `PyPDFLoader`
- Chunking and text splitting with `RecursiveCharacterTextSplitter`
- Vector embeddings with `GoogleGenerativeAIEmbeddings`
- Vector store with `Chroma`
- Retrieval-based question answering with `ChatGoogleGenerativeAI`
- Interactive Streamlit chat interface

---

## 📂 Project Structure
```
.
├── app.py                # Main Streamlit application
├── my_paper.pdf          # Your PDF file to query
├── requirements.txt      # Python dependencies
├── .env                  # Environment variables
└── README.md             # Documentation
```

---

## ⚙️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/your-username/rag-gemini-app.git
cd rag-gemini-app
```

### 2. Create virtual environment
```bash
python -m venv venv
source venv/bin/activate   # On Mac/Linux
venv\Scripts\activate      # On Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

---

## 📦 Requirements

Create a **requirements.txt** file with the following:

```txt
streamlit
langchain
langchain-community
langchain-google-genai
langchain-chroma
python-dotenv
```

---

## 🔑 Environment Variables
Create a `.env` file in the project root and add:

```ini
GOOGLE_API_KEY=your_google_api_key_here
```

---

## ▶️ Running the Application
```bash
streamlit run app.py
```

Then open your browser at `http://localhost:8501`.

---

## 📝 Usage
1. Place your PDF file (e.g., `my_paper.pdf`) in the project directory.
2. Run the app.
3. Type your question in the chat input.
4. Get answers retrieved from your PDF, powered by **Gemini Pro**.

---

## 📌 Example
Input:
```
What is the main contribution of this paper?
```

Output:
```
The paper introduces a novel approach to retrieval-augmented generation, 
leveraging embeddings and context retrieval to improve accuracy in question answering.
