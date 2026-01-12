🏥 Medical ChatBot using LangChain & Gemini

An AI-powered Medical ChatBot that answers health-related queries using LLMs + Vector Search.
It uses LangChain, Gemini, and Pinecone to provide accurate, context-aware responses.

📸 Project Preview

✨ Features

🧠 AI-powered medical question answering

📚 Contextual responses using Pinecone Vector DB

🔍 Retrieval-Augmented Generation (RAG)

🌐 Web interface built with Flask

🔐 Secure API key handling via .env

🛠 Tech Stack
Technology	Purpose
Python	Core language
LangChain	LLM orchestration
Gemini API	Large Language Model
Pinecone	Vector database
Flask	Web framework

📂 Project Structure
Medical_ChatBot/
│     
├── data/                   # Medical documents / PDFs used for embeddings
├── research/               # Experiments, notebooks, or R&D files
├── src/                    # Core source code (LLM, chains, helpers)
├── static/                 # Static files (CSS, JS, images)
├── templates/              # HTML templates for Flask UI
│
├── .env                    # Environment variables (API keys)
├── .gitignore              # Files ignored by Git
├── app.py                  # Main Flask application
├── store_index.py          # Embedding creation & Pinecone storage
├── requirements.txt        # Python dependencies
├── setup.py                # Package setup configuration
├── LICENSE                 # Project license
└── README.md               # Project documentation


🚀 How to Run the Project
🔹 STEP 1: Clone the Repository
git clone https://github.com/tushar-kanti26/Medical_ChatBot.git
cd Medical_ChatBot

🔹 STEP 2: Create & Activate Conda Environment
conda create -n medibot python=3.10 -y
conda activate medibot

🔹 STEP 3: Install Dependencies
pip install -r requirements.txt

🔹 STEP 4: Setup Environment Variables

Create a .env file in the root directory and add:

PINECONE_API_KEY="your_pinecone_api_key"
GEMINI_API_KEY="your_gemini_api_key"


⚠️ Never push .env to GitHub

🔹 STEP 5: Store Embeddings in Pinecone

Run once only (do not repeat unless data changes):

python store_index.py

🔹 STEP 6: Run the Application
python app.py

🔹 STEP 7: Open in Browser
http://localhost:5000

🧠 How It Works (High-Level)

Medical data is converted into embeddings

Embeddings are stored in Pinecone

User query → relevant context retrieved

Gemini generates a contextual response

🔐 Security Notes

API keys are loaded via .env

.env is excluded using .gitignore

No secrets are hardcoded
