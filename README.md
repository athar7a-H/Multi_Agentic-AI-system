<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Syne&weight=700&size=32&pause=1000&color=E8572A&center=true&vCenter=true&width=600&lines=ResearchMind+AI+%F0%9F%94%AC;Multi-Agent+Research+System;Search+%E2%86%92+Read+%E2%86%92+Write+%E2%86%92+Critique" alt="Typing SVG" />

<br/>

![Python](https://img.shields.io/badge/Python-3.10+-E8572A?style=for-the-badge&logo=python&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-0.1+-000000?style=for-the-badge&logo=chainlink&logoColor=white)
![Mistral AI](https://img.shields.io/badge/Mistral_AI-Small-FF7000?style=for-the-badge&logo=mistral&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-1.x-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge)

<br/>

> **Type any topic. Four autonomous AI agents take over.**
> They search the web, scrape the best sources, write a full research report,
> and critically review it — all before you finish your coffee.

<br/>

</div>

---

## 🧠 What Is This?

**ResearchMind AI** is a multi-agent research pipeline where four specialized AI agents collaborate in sequence to turn any topic into a fully structured, peer-reviewed research report — automatically.

No copy-pasting from browser tabs. No manual summarizing. No second-guessing your own writing. Just type a topic and watch the pipeline run.

---

## 🤖 Meet The Agents

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│   🔍 HUNTER  →  📖 READER  →  ✍️ WRITER  →  🎯 CRITIC          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

| Agent | Role | What It Does |
|-------|------|--------------|
| 🔍 **Hunter** | Search Agent | Crawls the live web for recent, reliable, cited sources on your topic |
| 📖 **Reader** | Reader Agent | Picks the richest URL from search results and scrapes it for deep content |
| ✍️ **Writer** | Writer Chain | Synthesizes everything into a structured report — intro, findings, conclusion, sources |
| 🎯 **Critic** | Critic Chain | Reads the report, scores it out of 10, lists strengths, weaknesses, and a final verdict |

---

## ✨ Features

- 🌐 **Live web search** — agents pull real, current information. No hallucinated facts
- 🕸️ **Deep URL scraping** — goes beyond snippets to extract actual page content
- 📝 **Structured reports** — every report has intro, key findings, conclusion, and sources
- 🎯 **AI peer review** — an independent critic agent scores and critiques before you see it
- 💻 **Stunning dark UI** — custom Streamlit dashboard with animated pipeline tracker
- 📟 **Live log terminal** — watch every agent step happen in real time
- ⚡ **Quick topic chips** — one-click preset topics to get started instantly
- 🔒 **Secure** — API keys stay local, never committed to version control

---

## 🖥️ UI Preview

```
┌──────────────────────────────────────────────────────────────────────┐
│  ⚡ Mistral · Multi-Agent Research System                            │
│                                                                      │
│           ResearchMind AI                                            │
│    Four autonomous agents. One definitive report.                    │
│                                                                      │
│  🔍 Search ──› 📖 Reader ──› ✍️ Writer ──› 🎯 Critic               │
├────────────────────┬─────────────────────────────────────────────────┤
│                    │                                                 │
│  Research Topic    │   🔍 Search Results          [ Agent 1 ]       │
│  ┌──────────────┐  │   ┌───────────────────────────────────────┐    │
│  │ Quantum AI…  │  │   │ Found 8 sources on Quantum AI...      │    │
│  └──────────────┘  │   └───────────────────────────────────────┘    │
│                    │                                                 │
│  Quick Topics      │   📖 Scraped Content         [ Agent 2 ]       │
│  [Quantum AI] ...  │   ┌───────────────────────────────────────┐    │
│                    │   │ Deep content from arxiv.org...        │    │
│  🚀 Run Pipeline   │   └───────────────────────────────────────┘    │
│                    │                                                 │
│  Live Log          │   ✍️ Research Report       [ Writer Chain ]    │
│  ▸ Searching...    │   ┌───────────────────────────────────────┐    │
│  ✓ Search done     │   │ ## Introduction                       │    │
│  ▸ Scraping...     │   │ ## Key Findings                       │    │
│                    │   │ ## Conclusion                         │    │
│                    │   └───────────────────────────────────────┘    │
│                    │                                                 │
│                    │   🎯 Critic Review          [ Complete ✓ ]     │
│                    │   ┌──────┐ ████████████░░░░ Score: 8/10        │
│                    │   │  8   │ Strengths / Areas to Improve        │
│                    │   └──────┘                                     │
└────────────────────┴─────────────────────────────────────────────────┘
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| 🧠 LLM | Mistral AI (`mistral-small-latest`) |
| 🔗 Agent Framework | LangChain |
| 🌐 Web Interface | Streamlit |
| 🔍 Search Tool | Custom `web_search` tool |
| 📖 Scraper Tool | Custom `scrape_url` tool |
| 🔐 Secrets | python-dotenv |
| 🐍 Language | Python 3.10+ |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/researchmind-ai.git
cd researchmind-ai
```

### 2. Create a virtual environment

```bash
python -m venv .venv

# Windows
.venv\Scripts\activate

# Mac/Linux
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up your API key

```bash
# Copy the example env file
cp .env.example .env
```

Open `.env` and add your real key:

```env
MISTRAL_API_KEY=your_mistral_api_key_here
```

Get your free Mistral API key at → **https://console.mistral.ai**

### 5. Run the app

```bash
streamlit run app.py
```

Open your browser at `http://localhost:8501` and start researching. 🎉

---

## 📁 Project Structure

```
researchmind-ai/
│
├── app.py              # Streamlit UI — dashboard, layout, pipeline execution
├── agents.py           # LangChain agents + writer & critic chains
├── pipeline.py         # Main pipeline orchestrator — runs all 4 agents
├── tools.py            # web_search and scrape_url tool definitions
│
├── .env                # 🔒 Your API keys (never committed)
├── .env.example        # Safe template for others to copy
├── .gitignore          # Keeps .env and venv out of Git
├── requirements.txt    # All dependencies
└── README.md           # This file
```

---

## 📦 Requirements

```txt
langchain
langchain-core
langchain-mistralai
streamlit
python-dotenv
```

---

## 🔐 Keeping Your Keys Safe

This project uses `python-dotenv` to load API keys from a local `.env` file.
The `.env` file is listed in `.gitignore` and will **never** be uploaded to GitHub.

✅ Safe to commit → `.env.example`, `agents.py`, `app.py`
❌ Never commit → `.env`, `.venv/`

---

## 🗺️ Roadmap

- [ ] Multi-turn refinement — agents loop and improve based on critic feedback
- [ ] PDF export of final report
- [ ] Agent debate mode — two writers, one judge
- [ ] Topic history and saved reports
- [ ] Support for more LLM providers (OpenAI, Gemini, Groq)
- [ ] Docker support for one-command deployment

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

<div align="center">

**Built with 🤝 human creativity + AI assistance**

*If this project helped you, consider giving it a ⭐ on GitHub!*

</div>
