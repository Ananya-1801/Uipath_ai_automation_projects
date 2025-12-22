# Stock Advisor Agent

The Stock Advisor Agent is a **prompt-driven AI automation project** developed using **UiPath Studio Web**.  
The agent analyzes provided stock-related data and generates a **Buy or Don't Buy recommendation** based solely on the information supplied at runtime.

---

## 📌 Project Description

This project implements an AI-powered stock recommendation assistant that evaluates stock information such as current price, historical performance, and relevant market indicators. The agent follows a predefined analytical prompt and does **not rely on external context files, indexes, or stored data**.

All recommendations are generated dynamically based on the input data provided during execution.

---

## 🧠 Agent Prompt Logic

The agent follows these guiding principles:

- Analyzes provided stock data, including:
  - Current price
  - Historical performance
  - Market indicators
- Considers factors such as:
  - Price-to-earnings (P/E) ratio
  - Market trends
  - Company fundamentals
  - Recent news (if available in input)
- Produces a clear:
  - **Buy** or **Don't Buy** recommendation
- Provides a concise, data-driven explanation
- Identifies insufficient data when applicable and specifies required inputs
- Always includes a disclaimer stating the recommendation is **for informational purposes only** and **not financial advice**

---

## ⚙️ Key Features

- Prompt-based decision analysis  
- No external context or memory dependency  
- JSON-based structured input handling  
- Objective and rule-guided recommendation output  
- Built entirely using UiPath Studio Web  

---

## 🛠️ Tools & Technologies

- UiPath Studio Web  
- UiPath Orchestrator  
- JSON  

---

## 📈 Outcome

- Demonstrates effective use of **prompt engineering** in automation  
- Highlights decision-making without persistent context  
- Ensures ethical handling of financial recommendations  
- Reinforces clarity, objectivity, and transparency in AI-driven analysis  

---

## 📂 Files Included

- `.uis` workflow file containing the Stock Advisor Agent logic
