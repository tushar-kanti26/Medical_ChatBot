# 🏥 Medical ChatBot

An AI-powered medical assistant designed to provide accurate information by leveraging Retrieval-Augmented Generation (RAG). This project uses **Gemini** for reasoning, **Pinecone** for vector search, and **LangChain** for orchestration, all wrapped in a sleek **Flask** web interface.

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
├── research/          # Experiments, notebooks, and R&D files
├── src/               # Core source code (LLM chains, helpers)
├── static/            # Frontend assets (CSS, JS, images)
├── templates/         # HTML templates for Flask UI
├── .env               # Environment variables (Private)
├── .gitignore         # Files ignored by Git
├── app.py             # Main Flask application
├── store_index.py     # Script to create & store embeddings
├── requirements.txt   # Python dependencies
├── setup.py           # Package setup configuration
└── LICENSE            # Project license

🚀 How to Run the Project
🔹 Step 1: Clone the Repository
git clone https://github.com/tushar-kanti26/Medical_ChatBot.git
cd Medical_ChatBot

🔹 Step 2: Create & Activate Conda Environment
conda create -n medibot python=3.10 -y
conda activate medibot

🔹 Step 3: Install Dependencies
pip install -r requirements.txt

🔹 Step 4: Setup Environment Variables

Create a .env file in the root directory:

PINECONE_API_KEY=your_pinecone_api_key
GEMINI_API_KEY=your_gemini_api_key

🔹 Step 5: Store Embeddings in Pinecone

⚠️ Run this only once (unless documents change):

python store_index.py

🔹 Step 6: Run the Application
python app.py

🔹 Step 7: Open in Browser
http://localhost:5000
