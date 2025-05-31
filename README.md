import { Callout } from 'nextra/components'
import Tabs from '@theme/Tabs'
import TabItem from '@theme/TabItem'

# 🧮 MathQueryAI-Agent

A smart AI-powered assistant built with **Streamlit**, **LangChain**, and **Google Gemma 2**, capable of solving complex text-based mathematical problems and searching Wikipedia for relevant information. This agent uses multiple tools — a calculator, logical reasoning chain, and a knowledge retriever — all orchestrated through a `zero-shot-react-description` LangChain agent.

---

## 🚀 Features

- 🧠 Converts real-world word problems into structured math problems and solves them step-by-step.
- 🌐 Wikipedia-powered research for context-aware knowledge support.
- 🤖 Agent-based architecture with reasoning and math tools.
- 🔐 Secure integration with Groq API for LLM access.
- ⚡ Interactive UI with Streamlit for real-time Q&A.

---

## 📁 Folder & File Structure

```bash
.
├── app.py                 # 🚀 Main entry point for Streamlit app
├── requirements.txt       # 📦 Python dependencies

