# 🤖 Testing Codestral for SQL & Python Generation

Hands-on experiments evaluating **Mistral's Codestral** model as an AI code assistant for two core data engineering tasks: **SQL query generation** and **Python code generation**.

---

## 📌 Overview

Codestral is a code-specialized LLM trained on 80+ programming languages. This repo benchmarks its practical usefulness for data professionals by testing it against realistic SQL and Python tasks — from simple queries to more complex data manipulation patterns.

The goal is to understand where Codestral excels, where it struggles, and how reliably it can be used as a coding co-pilot in data workflows.

---

## 📁 Repository Structure

```
├── Codestral_4_SQLGeneration.ipynb       # SQL generation experiments
├── Codestral_PythonCodeGeneration.ipynb  # Python code generation experiments
├── operations.py                         # Helper functions used across notebooks
├── __init__.py
└── README.md
```

---

## 🧪 Experiments

### 1. SQL Generation — `Codestral_4_SQLGeneration.ipynb`

Tests Codestral's ability to generate correct SQL from natural language prompts, covering:

- Basic `SELECT`, `WHERE`, `GROUP BY` queries
- Aggregations and window functions
- Multi-table `JOIN` patterns
- Filtering and sorting on realistic schemas

### 2. Python Code Generation — `Codestral_PythonCodeGeneration.ipynb`

Tests Codestral's ability to produce working Python code for data tasks, covering:

- Data manipulation with `pandas`
- Writing reusable functions
- Common scripting patterns for ETL workflows
- Code completion from partial implementations

---

## 🚀 Getting Started

### Prerequisites

```bash
pip install mistralai jupyter pandas
```

You will need a **Mistral API key**. Get one at [console.mistral.ai](https://console.mistral.ai).

### Setup

```bash
git clone https://github.com/alketcecaj12/TestingCodestral_4_SQLandPythonGeneration.git
cd TestingCodestral_4_SQLandPythonGeneration
```

Set your API key as an environment variable:

```bash
export MISTRAL_API_KEY="your_api_key_here"
```

Then open either notebook:

```bash
jupyter notebook Codestral_4_SQLGeneration.ipynb
```

---

## 🔑 Key Findings

| Task | Codestral Performance |
|---|---|
| Simple SQL queries | ✅ Reliable |
| Multi-table JOINs | ✅ Good with clear schema context |
| Window functions | ⚠️ Works with explicit hints |
| Python data wrangling | ✅ Reliable for standard patterns |
| Complex ETL logic | ⚠️ Requires prompt iteration |

---

## 🛠️ Tech Stack

- **Model**: [Codestral](https://mistral.ai/news/codestral/) by Mistral AI
- **Interface**: Mistral Python SDK
- **Environment**: Jupyter Notebooks
- **Language**: Python 3.x

---

## 📄 License

MIT License — free to use and adapt.

---

## 🙋 Author

**Alket Cecaj** — Data Scientist & Quantitative Analyst  
[GitHub](https://github.com/alketcecaj12)
