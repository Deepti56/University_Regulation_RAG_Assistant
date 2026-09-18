# 🎓 University Regulation RAG Assistant

A **Retrieval-Augmented Generation (RAG)** based AI assistant that answers questions from uploaded **university regulations, academic rules, examination guidelines, attendance policies, and student handbooks**.

## 🚀 Key Features

* 📄 Upload and process multiple PDF documents
* 🔍 Semantic search using vector embeddings
* ⚡ FAISS-based fast document retrieval
* 🤖 AI-generated answers using retrieved context
* 📌 Provides **document and page citations**
* 🛡️ Reduces hallucinations using context-only answering
* 💬 Interactive Gradio chatbot interface

## 🏗️ RAG Workflow

```text
PDF Documents
      ↓
Text Extraction
      ↓
Text Chunking
      ↓
Sentence Transformer Embeddings
      ↓
FAISS Vector Database
      ↓
Relevant Document Retrieval
      ↓
FLAN-T5
      ↓
Answer + Sources
```

## 🛠️ Technologies

* Python
* Google Colab
* PyPDF
* Sentence Transformers
* FAISS
* FLAN-T5
* Gradio

## ⚙️ Main Configuration

```text
Chunk Size: 500 characters
Chunk Overlap: 100 characters
Embedding Model: all-MiniLM-L6-v2
Embedding Dimension: 384
Top-K Retrieval: 5
Similarity Threshold: 0.30
LLM: google/flan-t5-base
```

## 📊 Example

**Question:**

> What is the minimum attendance required for the end-semester examination?

**Answer:**

> 75%

The system also displays the **source PDF, page number, and similarity score**.

## 🛡️ Hallucination Control

The assistant is instructed to answer **only from the uploaded documents**. If the required information is not available, it responds:

> “Information not found in the uploaded university documents.”

## 📁 Project Structure

```text
University-Regulation-RAG/
│
├── University_Regulation_RAG_Assistant_Colab.ipynb
├── requirements.txt
├── README.md
└── data/
    └── university_pdfs/
```

## 🔮 Future Enhancements

* Web-based deployment
* Support for more document formats
* Multilingual university support
* Improved citation and source highlighting
* Advanced reranking for better retrieval

## 👩‍💻 Author

**Deepti Karalapati**

B.Tech CSE (AI & ML)

231FA18309
