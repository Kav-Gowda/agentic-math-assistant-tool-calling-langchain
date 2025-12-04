# 🧮 Agentic Math Assistant with Tool Calling (LangChain + LangGraph)

This project implements a fully agentic Math Assistant using LangChain, LangGraph, and open-source LLMs.  
The assistant can parse natural language queries, call mathematical tools, combine reasoning with retrieval, and return structured answers.  
Everything runs on Google Colab without API keys.

This repository is part of my Agentic AI Engineering portfolio.

---

## 🚀 Project Highlights

### 1. Mathematical Tool Suite
The assistant includes several tools, each implemented with LangChain’s @tool decorator:

- add_numbers  
- new_subtract_numbers  
- multiply_numbers  
- divide_numbers  
- sum_numbers_from_text  
- sum_numbers_with_complex_output  

Each tool provides structured inputs and outputs, enabling predictable agent behavior.

---

### 2. Agentic ReAct Reasoning (LangGraph)
Using LangGraph’s prebuilt ReAct agent, the assistant:

- Understands user intent  
- Selects the correct tool  
- Executes operations  
- Returns a final answer with reasoning steps  

This demonstrates practical agent orchestration and tool-enabled decision making.

---

### 3. Advanced Subtraction Logic
Two subtraction tools are compared:

- subtract_numbers → negates the first input then subtracts  
- new_subtract_numbers → performs intuitive sequential subtraction  

This showcases design decisions behind mathematical tool behavior.

---

### 4. Wikipedia Integration
A factual lookup tool is included:

- search_wikipedia(query: str)

This allows hybrid workflows like:

> “What is the population of Canada? Multiply it by 0.75.”

The agent performs retrieval + numerical reasoning together.

---

### 5. Built-in Testing Framework
The notebook includes custom tests that:

- Evaluate whether the agent selects the correct tool  
- Compare tool results to expected values  
- Validate the agent’s reliability in mixed scenarios  

---

## 📂 Repository Structure

    agentic-math-assistant-tool-calling-langchain/
    ├── agentic_math_assistant_tool_calling_langchain.ipynb   # Main notebook
    ├── README.md                                             # Project documentation
    ├── requirements.txt                                      # Dependencies
    ├── .gitignore                                            # Git ignore rules
    └── LICENSE                                               # MIT License

---

## 🛠️ Tech Stack

- LangChain (tools, schemas, agents)  
- LangGraph (ReAct workflow execution)  
- HuggingFace Transformers (open-source LLM)  
- WikipediaAPIWrapper  
- Python 3.10+  
- Google Colab  

No paid APIs required.

---

## ▶️ How to Run

1. Clone the repository:

       git clone https://github.com/<your-username>/agentic-math-assistant-tool-calling-langchain.git
       cd agentic-math-assistant-tool-calling-langchain

2. Open the notebook in **Google Colab**.

3. Run the installation cell.

4. Execute all sections to explore tool calling, agent reasoning, and evaluation tests.

---

## 📘 Workflows Demonstrated

- Natural-language math interpretation  
- Tool selection via agent reasoning  
- Multi-tool orchestration  
- Sequential and parallel numerical operations  
- Retrieval-augmented computation (Wikipedia + math)  

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 💬 Author

**Kavitha Lingarajegowda**  
Agentic AI Engineering | LLM Systems | Automotive AI  
LinkedIn | Portfolio
