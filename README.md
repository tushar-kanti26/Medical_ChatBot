# 🏥 Medical ChatBot

An AI-powered medical assistant designed to provide accurate information by leveraging Retrieval-Augmented Generation (RAG). This project uses **Gemini** for reasoning, **Pinecone** for vector search, and **LangChain** for orchestration, all wrapped in a sleek **Flask** web interface.

---

## 🖼️ Project Screenshots

### **Chatbot Interface**
| User Conversation | AI Response |
| :---: | :---: |
| ![Chatbot 1](Screenshots/chatbot1.png) | ![Chatbot 2](Screenshots/coding.png) |

<br>

### **Vector Database (Pinecone)**
<p align="center">
  <img src="screenshots/pinecone_db.png" width="800" alt="Pinecone Index">
  <br>
  <em>Visualizing medical document embeddings stored in Pinecone</em>
</p>

---

## 🌟 Features

* **RAG Integration:** Uses Pinecone to retrieve relevant medical context before generating answers.
* **LLM Powered:** Utilizes Google’s Gemini API for high-quality conversational responses.
* **Vector Storage:** Efficiently stores and searches medical document embeddings.
* **Web UI:** A user-friendly interface built with Flask, HTML, and CSS.
* **Security First:** Environment variable management to protect sensitive API keys.

---

## 🛠 Tech Stack

| Technology | Purpose |
| :--- | :--- |
| **Python** | Core programming language |
| **LangChain** | LLM orchestration and RAG framework |
| **Gemini API** | Large Language Model (Google) |
| **Pinecone** | Vector database for similarity search |
| **Flask** | Web framework for the frontend |

---

## 📂 Project Structure

```text
Medical_ChatBot/
├── data/              # Medical documents / PDFs for embeddings
├── screenshots/       # Project images (Chatbot and Pinecone)
├── src/               # Core source code (LLM chains, helpers)
├── static/            # Frontend assets (CSS, JS, images)
├── templates/         # HTML templates for Flask UI
├── .env               # Environment variables (Private)
├── app.py             # Main Flask application
├── store_index.py     # Script to create & store embeddings
├── requirements.txt   # Python dependencies
└── README.md          # Documentation
