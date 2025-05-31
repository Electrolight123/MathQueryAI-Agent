<div align="center">
# 🧮 MathQueryAI-Agent
</div>

<p align="center">
  <a href="https://streamlit.io/">
    <img src="https://img.shields.io/badge/Made%20With-Streamlit-ff4b4b.svg?style=flat-square" alt="Streamlit" />
  </a>
  <a href="https://python.org">
    <img src="https://img.shields.io/badge/Python-3.9+-blue.svg?style=flat-square" alt="Python" />
  </a>
  <a href="https://github.com/langchain-ai/langchain">
    <img src="https://img.shields.io/badge/LangChain-Enabled-brightgreen.svg?style=flat-square" alt="LangChain" />
  </a>
  <a href="https://github.com/Electrolight123/MathQueryAI-Agent/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/Electrolight123/MathQueryAI-Agent?style=flat-square" alt="License" />
  </a>
</p>

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

```

---

## 📦 Installation

### 1. Clone the repository
```bash
git clone https://github.com/your-username/MathQueryAI-Agent.git
cd MathQueryAI-Agent
```
### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```
### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the app
```bash
streamlit run app.py
```

---

## 🔑 Configuration

You must enter your **Groq API Key** in the sidebar when prompted to access the Gemma 2 LLM.

> 🔐 **Groq API Key** is required for the LLM to function. The app won’t proceed without it.

---

## 🧠 How It Works
The app initializes an agent with three powerful tools:

### 📚 Wikipedia Tool
- Uses WikipediaAPIWrapper to fetch topic summaries.

### ➕ Calculator Tool
- Uses LLMMathChain to solve numeric problems.

### 💡 Reasoning Tool
- Custom PromptTemplate and LLMChain to solve logic-based queries.

Once a user inputs a question, the agent selects the most appropriate tool (or combination) to generate a clear, step-by-step answer using Gemma 2 LLM hosted by Groq.

---

## ✍️ Usage Example

```css
I have 5 bananas and 7 grapes. I eat 2 bananas and give away 3 grapes. 
Then I buy a dozen apples and 2 packs of blueberries. Each pack of blueberries contains 25 berries. 
How many total pieces of fruit do I have at the end?
```

✅ The assistant parses the logic, performs calculations, and returns:

> 🧮 Final Count: 67 fruits
> 📝 Step-by-step explanation (pointwise)

---

## 👨‍💻 Technologies Used

| Tool              | Purpose                               |
| ----------------- | ------------------------------------- |
| 🟣 Streamlit      | Web App UI                            |
| 🧠 LangChain      | Agent management & tool orchestration |
| 🟡 Groq (Gemma 2) | LLM backend                           |
| 📚 Wikipedia API  | Knowledge retrieval                   |
| ➗ LLMMathChain    | Math problem solving                  |

---

## 🙌 Contributing

Contributions are welcome! 🚀

>1. Fork the repo
> 2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
> 3. Commit your changes (`git commit -m 'Add amazing feature'`)
> 4. Push to the branch (`git push origin feature/AmazingFeature`)
> 5. Open a pull request

---

## 🪪 License

This project is licensed under the **MIT License** — see the [LICENSE]([https://github.com/Electrolight123/MathQueryAI-Agent/blob/main/LICENSE]) file for details.

---

> 💡 **Tip**: Want to use your own LLM backend? Just replace the `ChatGroq` wrapper with another LangChain-compatible LLM in `app.py`. 
