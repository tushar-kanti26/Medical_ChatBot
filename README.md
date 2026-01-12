🏥 Medical ChatBot

An AI-powered medical chatbot built using LangChain, Gemini, and Pinecone, with a Flask-based web interface.

🔐 Security

Secure API key handling using .env

No secrets committed to GitHub

🛠 Tech Stack
Technology	Purpose
Python	Core programming language
LangChain	LLM orchestration
Gemini API	Large Language Model
Pinecone	Vector database
Flask	Web framework
📂 Project Structure
Medical_ChatBot/
│
├── data/                 # Medical documents / PDFs used for embeddings
├── research/             # Experiments, notebooks, or R&D files
├── src/                  # Core source code (LLM, chains, helpers)
├── static/               # Static files (CSS, JS, images)
├── templates/            # HTML templates for Flask UI
│
├── .env                  # Environment variables (API keys)
├── .gitignore            # Files ignored by Git
├── app.py                # Main Flask application
├── store_index.py        # Embedding creation & Pinecone storage
├── requirements.txt      # Python dependencies
├── setup.py              # Package setup configuration
├── LICENSE               # Project license
└── README.md             # Project documentation

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
