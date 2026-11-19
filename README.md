# AI_CHATBOT_USING_RAG
An interactive AI chatbot built with Python, Streamlit, LangChain, and Groq for fast, real-time conversational responses with persistent chat history.
# AI Chatbot

A fast, interactive conversational AI chatbot built with **Streamlit**, **LangChain**, and **Groq**. It delivers real-time responses powered by large language models and maintains full conversation history within your browser session.

## Features
- **Interactive Chat UI:** Clean, responsive chat interface built with Streamlit (`st.chat_input` and `st.chat_message`).
- **Session Memory:** Keeps track of your ongoing conversation using Streamlit's `session_state`.
- **Ultra-Fast Inference:** Powered by Groq's low-latency LLM API (`llama-3.3-70b-versatile`).
- **Custom Prompting:** Uses LangChain prompt templates (`ChatPromptTemplate`) to guide the assistant's tone and response style.
- **Secure Key Management:** Loads API credentials safely from a local `.env` file.

## Tech Stack
- **Frontend:** Streamlit
- **Orchestration:** LangChain (`langchain-groq`, `langchain-core`)
- **LLM Provider:** Groq API
- **Environment Management:** `python-dotenv` / `pipenv`

## Project Structure
```text
├── Phase1.py        # Main Streamlit chatbot application
├── .env             # Environment variables (not tracked by Git)
└── README.md        # Project documentation
```

## Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com
   cd your-repo-name
   ```

2. **Install dependencies:**
   ```bash
   pip install streamlit langchain-groq langchain-core python-dotenv
   ```
   *(Or if using `pipenv`: `pipenv install`)*

3. **Configure your API key:**
   Create a `.env` file in the root directory and add your Groq API key:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

4. **Run the application:**
   ```bash
   streamlit run Phase1.py
   ```
Check out the website: https://aichatbotusingrag.streamlit.app/
## Usage
1. Open the local URL provided in your terminal (usually `http://localhost:8501`).
2. Type your question or message into the chat input box at the bottom.
3. Press **Enter** to receive an instant response from the AI assistant.
<img width="1114" height="702" alt="Screenshot 2026-11-18 214410" src="https://github.com/user-attachments/assets/45d5a89f-a130-45b1-acde-38a54dca7752" />

