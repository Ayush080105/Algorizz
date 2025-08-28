# Algorizz RAG Chatbot 🤖📄

This is a Retrieval-Augmented Generation (RAG) chatbot built with **Gradio** and deployed on Hugging Face Spaces.
You can upload your PDFs and ask questions, and the chatbot will retrieve relevant context before generating an answer.
The link to the deployed space: https://huggingface.co/spaces/Ayush0716/Algorizz

---

## 🚀 Features

* 📂 Upload and index PDF documents
* 🔍 Context-aware question answering with RAG
* 🧠 **Conversation Memory** — the chatbot remembers previous interactions in the session
* 🤖 Powered by **LLMs** (OpenAI / HuggingFace models)
* 🎨 Simple and clean **Gradio interface**
* 🌐 Deployable seamlessly on **Hugging Face Spaces**

---

## 🛠️ Installation (Run Locally)

Clone the repository:

```bash
git clone https://huggingface.co/spaces/Ayush0716/Algorizz_Rag_Chatbot
cd Algorizz_Rag_Chatbot
```

Create a virtual environment and activate it:

```bash
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the app:

```bash
python app.py
```

---

## 📦 Deployment on Hugging Face Spaces

This repo already includes:

* `app.py` → main Gradio app
* `requirements.txt` → dependencies
* `README.md` → Space metadata & instructions

To update your Space:

```bash
git add .
git commit -m "Update app"
git push hf main
```

Hugging Face will automatically rebuild and relaunch the Space.

---

## ⚙️ Requirements

Inside `requirements.txt` (example):

```
gradio
langchain
langchain-community
langchain-openai
faiss-cpu
sentence-transformers
pypdf
openai
```

---

## 🔮 Future Scope

* 📝 **Fallback OCR support** for scanned or image-based PDFs (using Tesseract, PaddleOCR, or Hugging Face OCR models).
* 🌐 **Web/Tool Augmentation**:

  * SERP APIs for real-time search queries.
  * **MCP (Model Context Protocol)** or Playwright integration for structured web browsing & interaction.
* 🔧 **Advanced memory** persistence across sessions (database-backed).
* 📊 Multi-modal support (images, tables, charts inside PDFs).

---

## 🙌 Acknowledgements

* [Gradio](https://gradio.app/) for the UI
* [LangChain](https://www.langchain.com/) for RAG pipeline + memory
* [Hugging Face Spaces](https://huggingface.co/spaces) for deployment
