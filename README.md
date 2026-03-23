# 🧠 Deep Research AI Agent

An end-to-end **multi-agent AI system** that performs deep research on any user query by planning, searching, summarizing, and delivering results via email.

---

## 🚀 Overview

This project implements an **autonomous research pipeline** using multiple AI agents.
It takes a user query and:

1. Plans what to search
2. Fetches real-time information from the web
3. Synthesizes a detailed report
4. Sends the report via email

---

## 🏗️ Architecture

```
User Input (Gradio UI)
        ↓
ResearchManager (Orchestrator)
        ↓
Planner Agent 🧠
        ↓
Search Agent 🔍 (Parallel Execution)
        ↓
Writer Agent ✍️
        ↓
Email Agent 📧
        ↓
SendGrid API → Email Delivered
```

---

## ⚙️ Features

* ✅ Multi-agent architecture (Planner, Search, Writer, Email)
* ✅ Real-time web search using tools
* ✅ Parallel execution using `asyncio`
* ✅ Structured outputs using Pydantic
* ✅ Automated report generation (1000+ words)
* ✅ Email delivery using SendGrid
* ✅ Live progress updates via Gradio UI
* ✅ Tracing support for debugging workflows

---

## 🧩 Agents Description

### 🧠 Planner Agent

* Breaks down user query into multiple search queries
* Generates structured search plan with reasoning

### 🔍 Search Agent

* Uses `WebSearchTool` to fetch real-time data
* Summarizes results concisely

### ✍️ Writer Agent

* Combines all search results
* Generates a detailed markdown report
* Provides summary and follow-up questions

### 📧 Email Agent

* Converts report into HTML format
* Sends email using SendGrid API

---

## 📁 Project Structure

```
deep_research/
│
├── deep_research.py       # Gradio UI entry point
├── research_manager.py    # Orchestrates full pipeline
├── planner_agent.py       # Planning agent
├── search_agent.py        # Web search agent
├── writer_agent.py        # Report generation agent
├── email_agent.py         # Email sending agent
├── .env                   # Environment variables (not uploaded)
```

---

## 🛠️ Tech Stack

* Python (Asyncio)
* OpenAI Agents SDK
* Pydantic (Structured Outputs)
* SendGrid (Email API)
* Gradio (UI Interface)

---

## 🔧 Setup Instructions

### 1️⃣ Clone Repository

```bash
git clone https://github.com/Pranshu223/deep-research-agent.git
cd deep-research-agent
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Create `.env` File

```
OPENAI_API_KEY=your_openai_api_key
SENDGRID_API_KEY=your_sendgrid_api_key
```

---

### 4️⃣ Run Project

```bash
python deep_research.py
```

---

## 📊 Example Workflow

Input:

```
Latest AI agent frameworks in 2025
```

Output:

* Planned search queries
* Summarized web results
* Detailed research report
* Email delivered with report

---

## 🔥 Key Concepts Used

* Multi-Agent Systems
* Tool Calling
* Async Parallel Execution
* Structured Output (Pydantic)
* LLM Orchestration
* Streaming UI

---

## 🚀 Future Improvements

* Add memory for past research
* Implement guardrails for safety
* Support multiple LLM providers (Groq, Ollama)
* Deploy as web app

---

## 👨‍💻 Author

Built as part of learning advanced **AI Agent Systems & Backend Development**

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!

---
