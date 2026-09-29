# 🤖 LangGraph ReAct Agent with Gemini + Tavily

A conversational AI agent built with **LangGraph**, **Google Gemini**, and **Tavily Search** — capable of reasoning, searching the web in real-time, and answering questions accurately.

## 🧠 How It Works

This project implements a **ReAct (Reason + Act)** agent using the LangGraph framework:

1. **User asks a question**
2. **Gemini thinks** about what tool to use
3. **Tavily searches** the web for real-time information
4. **Gemini synthesizes** the result into a final answer

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| [LangGraph](https://github.com/langchain-ai/langgraph) | Agent orchestration (ReAct loop) |
| [Google Gemini 1.5 Flash](https://ai.google.dev/) | LLM reasoning |
| [Tavily Search](https://tavily.com/) | Real-time web search |
| [LangChain](https://langchain.com/) | LLM integrations |

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/YOUR_USERNAME/langchain-project.git
cd langchain-project
```

### 2. Create a virtual environment
```bash
python -m venv .venv
.venv\Scripts\activate   # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Set up environment variables
Create a `.env` file in the root directory:
```env
GEMINI_API_KEY=your_gemini_api_key
TAVILY_API_KEY=your_tavily_api_key
```

Get your keys:
- Gemini API Key → [Google AI Studio](https://aistudio.google.com/app/apikey)
- Tavily API Key → [Tavily](https://app.tavily.com)

### 5. Run the notebook
Open `agent.ipynb` in Jupyter and run all cells.

## 📁 Project Structure

```
langchain-project/
├── agent.ipynb          # Main notebook with agent code
├── requirements.txt     # Python dependencies
├── .env                 # API keys (DO NOT commit)
├── .gitignore           # Excludes .env and .venv
└── README.md            # This file
```

## 📦 Requirements

See [`requirements.txt`](requirements.txt) for the full list of dependencies.

## 🔒 Security

- **Never commit your `.env` file** — it's excluded by `.gitignore`
- Keep your API keys private

## 📄 License

MIT License — feel free to use and modify.
