

---

# ⚡ Energy Action Planner (GenAI + LangChain)

A lightweight **energy management simulation system** built using **Python and LangChain**, designed to demonstrate how **LLM-powered agents** can analyze energy usage, forecast demand, and recommend optimization strategies.

This project showcases how **Generative AI can be applied to real-world infrastructure problems** like smart grids and energy optimization.

---

## 🚀 Features

* 🔍 **Energy Usage Analysis**

  * Simulates daily energy consumption for a given location

* 📈 **Demand Forecasting**

  * Predicts next week’s energy demand using mock data

* 🧠 **AI-Based Recommendations**

  * Suggests optimization strategies based on forecast insights

* 🤖 **LangChain Agent Integration**

  * Uses ReAct-style agents for tool-based reasoning (API mode)

* 🧪 **Offline Demo Mode**

  * Fully functional without API keys (great for testing & demos)

---

## 🏗️ Architecture Overview

```
User Input (Location)
        ↓
[EnergyUsageAnalyzer Tool]
        ↓
[EnergyDemandForecaster Tool]
        ↓
[EnergyActionRecommender Tool]
        ↓
Final Optimization Recommendation
```

When API is enabled:

```
LangChain Agent (ReAct)
        ↓
Tool Selection + Reasoning
        ↓
Final Answer
```

---

## 📂 Project Structure

```
energy.py        # Main application script
README.md        # Project documentation
```

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/energy-action-planner.git
cd energy-action-planner
```

### 2. Install Dependencies

```bash
pip install langchain langchain-openai
```

---

## 🔑 Environment Setup (Optional - API Mode)

To enable full agent capabilities:

```bash
export OPENAI_API_KEY="your-api-key"
```

If not set, the project automatically runs in **demo mode**.

---

## ▶️ Usage

### Run the Application

```bash
python energy.py
```

### Sample Output

```
--- ENERGY ACTION PLANNER DEMO START (2026-04-16) ---

Step 1: Analyzing current energy usage...
Result: Energy usage in Bangalore is 532 kWh today.

Step 2: Forecasting energy demand...
Result: Forecasted energy demand for next week in Bangalore is 945 kWh.

Step 3: Getting optimization recommendations...
Result: Recommendation: Enable smart grid load balancing and add solar input.

Energy optimization analysis complete!
```

---

## 🧠 How It Works

### Tools

| Tool Name               | Description                    |
| ----------------------- | ------------------------------ |
| EnergyUsageAnalyzer     | Simulates current energy usage |
| EnergyDemandForecaster  | Predicts future demand         |
| EnergyActionRecommender | Suggests optimization actions  |

### Decision Logic

* If forecasted demand > 900 kWh:
  → Suggests **load balancing + solar integration**
* Otherwise:
  → Maintain current configuration

---

## 🤖 GenAI Integration

* Uses **LangChain Agents (ReAct pattern)** for:

  * Tool selection
  * Multi-step reasoning
* Falls back to a **manual execution pipeline** when API is unavailable

---

## 📌 Use Cases

* Smart grid optimization demos
* GenAI + backend engineering portfolio projects
* Energy analytics prototypes
* Interview-ready AI system design example

---

## 🛠️ Tech Stack

* Python
* LangChain
* OpenAI (optional)
* ReAct Agent Framework

---

## 🔮 Future Improvements

* Replace mock data with real energy datasets (e.g., IoT sensors)
* Add REST API (FastAPI) for production usage
* Integrate vector database for historical trend analysis
* Build dashboard (Streamlit / React)
* Add multi-location comparative analytics

---


