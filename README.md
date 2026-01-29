📄 Ask Your Document - Multi-Document ChatBot
A powerful, conversational AI application that allows users to upload multiple documents (PDF, DOCX, TXT) and have interactive conversations about their content. This app leverages LangChain, Groq (Llama 3), and FAISS for efficient retrieval and intelligent responses.

🚀 Features
Multi-Format Support: Upload and analyze .pdf, .docx, and .txt files simultaneously.

Conversational Memory: Remembers previous interactions for a natural chat experience.

High Performance: Powered by the Llama3-70b model via Groq for near-instant responses.

Local Vector Storage: Uses FAISS for fast and efficient document similarity search.

User-Friendly Interface: Built with Streamlit for a sleek, responsive UI.

🛠️ Tech Stack
Frontend: Streamlit

LLM Orchestration: LangChain

LLM: Groq (Llama 3 70B)

Embeddings: HuggingFace (all-MiniLM-L6-v2)

Vector Database: FAISS

Document Parsing: PyPDF2, docx2txt

📋 Prerequisites
Before running the project, ensure you have:

Python 3.9+ installed.

A Groq API Key (Get it at console.groq.com).

⚙️ Installation & Setup
Clone the repository:

Bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
Install dependencies:

Bash
pip install -r requirements.txt
Set up Secrets: Create a .streamlit/secrets.toml file in the root directory and add your Groq API key:

Ini, TOML
GROQ_API_KEY = "your_groq_api_key_here"
Alternatively, you can set it as an environment variable.

🏃 Running the App
Start the Streamlit server by running:

Bash
streamlit run app.py

