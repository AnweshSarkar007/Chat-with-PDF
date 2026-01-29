
# 📄 Ask Your Document

### Multi-Document Conversational Chatbot

**Ask Your Document** is an intelligent, conversational AI application that lets users upload **multiple documents** and chat with them in real time.
It supports **PDF, DOCX, and TXT** files and delivers fast, accurate answers using **state-of-the-art LLMs and vector search**.

Built for speed, simplicity, and scalability 🚀

---

## ✨ Key Features

* 📚 **Multi-Document Support**
  Upload and query multiple files at once (`.pdf`, `.docx`, `.txt`).

* 💬 **Conversational Memory**
  Maintains chat history for natural, context-aware conversations.

* ⚡ **High-Performance LLM**
  Powered by **Llama 3 (70B)** via **Groq** for ultra-fast responses.

* 🔍 **Semantic Search with FAISS**
  Efficient document retrieval using local vector similarity search.

* 🧠 **Accurate Embeddings**
  Uses HuggingFace’s `all-MiniLM-L6-v2` for high-quality embeddings.

* 🎨 **Clean & Interactive UI**
  Built with **Streamlit** for a smooth user experience.

---

## 🧰 Tech Stack

| Layer                | Technology                       |
| -------------------- | -------------------------------- |
| Frontend             | Streamlit                        |
| LLM Orchestration    | LangChain                        |
| Large Language Model | Groq 	                          |
| Embeddings           | HuggingFace                      |
| Vector Database      | FAISS                            |
| Document Parsing     | PyPDF2, docx2txt                 |

---

## 📦 Supported File Types

* 📄 PDF (`.pdf`)
* 📝 Word Documents (`.docx`)
* 📃 Text Files (`.txt`)

---

## 🔧 Prerequisites

Make sure you have:

* **Python 3.9+**
* **Groq API Key**

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure API Key

Create a secrets file:

```bash
.streamlit/secrets.toml
```

Add your Groq API key:

```toml
GROQ_API_KEY = "your_groq_api_key_here"
```

👉 Alternatively, you can set it as an environment variable:

```bash
export GROQ_API_KEY="your_groq_api_key_here"
```

---

## ▶️ Running the Application

Start the Streamlit app with:

```bash
streamlit run app.py
```

Once running, open your browser and start chatting with your documents 🎉

---

## 🧠 How It Works

1️⃣ **Upload Documents**
Users upload one or more documents via the sidebar.

2️⃣ **Text Extraction**
Content is extracted using format-specific loaders.

3️⃣ **Chunking**
Text is split into smaller, manageable chunks.

4️⃣ **Embedding Generation**
Each chunk is converted into vectors using HuggingFace embeddings.

5️⃣ **Vector Storage**
Embeddings are stored locally using FAISS.

6️⃣ **Question Answering**
User queries are matched semantically and answered using Llama 3.

---

## 📜 License

This project is licensed under the **MIT License**.

---

