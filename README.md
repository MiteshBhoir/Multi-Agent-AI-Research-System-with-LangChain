# 🔬 ResearchMind — Multi-Agent AI Research System

ResearchMind is an AI-powered research assistant that uses a **multi-agent architecture** to automatically gather, analyze, and generate structured research reports on any topic.

Instead of relying on a single LLM, this system uses **four specialized agents** that collaborate like a real research team:

* 🔍 Search Agent → Finds relevant web information
* 📄 Reader Agent → Extracts deep content from sources
* ✍️ Writer Agent → Generates structured research reports
* 🧐 Critic Agent → Reviews and scores the report

---

## 🚀 Features

* Multi-agent AI pipeline using LangChain
* Real-time web search using Tavily API
* Web scraping with BeautifulSoup
* Structured report generation (Introduction, Findings, Conclusion, Sources)
* Automated report evaluation with scoring & feedback
* Clean and modern UI built with Streamlit

---

## 🧠 Architecture
```
    User Input
            ↓
    Search Agent (web search)
            ↓
    Reader Agent (scraping)
            ↓
    Writer Chain (report generation)
            ↓
    Critic Chain (evaluation)
            ↓
    Final Output
```
---

## 📂 Project Structure

```
multiagent_ai/
│── app.py              # Streamlit frontend UI
│── agents.py           # Agent definitions (search + reader)
│── tools.py            # Custom tools (web search, scraping)
│── requirements.txt    # Dependencies
│── .env                # API keys (not committed)
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository

```
git clone https://github.com/your-username/multiagent-ai.git
cd multiagent-ai
```

---

### 2. Create virtual environment

```
python -m venv venv
venv\Scripts\activate        # Windows
# OR
source venv/bin/activate     # Mac/Linux
```

---

### 3. Install dependencies

```
pip install -r requirements.txt
```

---

### 4. Setup environment variables

Create a `.env` file in the root directory:

```
TAVILY_API_KEY=your_key
MISTRAL_API_KEY=your_key
# (Optional if using OpenAI)
OPENAI_API_KEY=your_key
```

---

## ▶️ Run the App

```
streamlit run app.py
```

App will be available at:

```
http://localhost:8501
```

---

## 🌐 Deployment

### ✅ Streamlit Cloud (Recommended)

1. Push code to GitHub
2. Go to https://share.streamlit.io
3. Select your repo and `app.py`
4. Add secrets:

   * `TAVILY_API_KEY`
   * `MISTRAL_API_KEY`

---

### ⚠️ Notes

* Do NOT upload:

  * `venv/`
  * `.env`
  * `__pycache__/`

* Make sure `requirements.txt` is included

---

## 🧪 Example Topics

* LLM Agents in 2025
* CRISPR Gene Editing
* Fusion Energy Progress
* AI in Healthcare

---

## 🛠️ Tech Stack

* Python
* Streamlit
* LangChain
* Mistral / OpenAI LLMs
* Tavily Search API
* BeautifulSoup
* Requests

---

## 🔮 Future Improvements

* FastAPI backend for scalability
* React frontend (production UI)
* Streaming responses
* Multi-document research
* Memory & chat history
* Parallel agent execution

---

## 👨‍💻 Author

MITESH BHOIR

---

## ⭐ Contribute

Feel free to fork this repo, improve it, and submit a PR!

---

## 📜 License

This project is open-source and available under the MIT License.
