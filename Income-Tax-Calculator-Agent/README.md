# 💼 Income Tax Calculation & Advisory Agent (FY 2025–26)

## 📌 Project Overview
The **Income Tax Calculation & Advisory Agent** is a context-grounded AI agent built using **UiPath Studio Web**.  
It assists users in **computing income tax liability for FY 2025–26** and provides **policy-aligned explanations** based strictly on **Indian Income Tax rules and slabs** applicable for the assessment year.

The agent ensures **accuracy, consistency, and transparency** by grounding all responses in **official tax policy documents and rule datasets**, avoiding assumptions or generic financial advice.

---

## 🎯 Objectives
- Calculate income tax liability for FY 2025–26
- Apply correct tax slabs and deductions
- Ensure compliance with applicable tax regimes
- Provide clear, explainable tax computation
- Prevent AI hallucinations using **context grounding**

---

## 🧠 Key Concept: Context Grounding
Context grounding ensures that the AI agent uses **only authoritative tax policy data** while answering queries.

In this project:
- Tax rules and slabs are stored in **Storage Buckets**
- Relevant policy files are indexed using **UiPath Indexes**
- The AI agent retrieves information **only from these indexes**
- User income details are passed dynamically at runtime

This guarantees:
- ❌ No outdated tax rules  
- ❌ No inferred deductions  
- ✅ Fully auditable and explainable tax results  

---

## 🏗️ Solution Architecture

User Income Details (Arguments / App)

Tax Policy Documents (Storage Bucket)

Policy Index (Context Grounding)

Income Tax AI Agent

Tax Liability Calculation + Explanation


---

## 🧩 Components Used

### 🔹 UiPath Services
- UiPath Studio Web
- UiPath Agents
- Storage Buckets
- Indexes
- Excel Integration

### 🔹 AI Capabilities
- Context-grounded retrieval
- Rule-based tax reasoning
- Policy-restricted responses

---


---

## 📊 Datasets Used

### 1️⃣ Tax_Slabs_FY2025_26.xlsx
Contains official income tax slabs and rates:
- Income ranges
- Tax percentages
- Regime applicability (Old / New)

> This file is uploaded to a **Storage Bucket** and indexed for grounding.


## 📚 Index Configuration

- **Index Name:** `Tax_Index`
- **Source:** Tax policy Excel files
- **Purpose:** Provide authoritative tax rules and slabs to the agent

Only policy documents are indexed; user income data is excluded.

---

## 🤖 Agent Prompt Design

### 🔐 System Prompt
Defines strict guardrails to ensure:
- Only indexed tax policies are used
- No assumptions about deductions or rebates
- Clear explanation of tax computation steps

### 🧑‍💼 User Prompt
Accepts runtime inputs such as:
- Annual income
- Selected tax regime
- Eligible deductions

And instructs the agent to:
- Compute tax liability
- Explain slab-wise calculation
- Cite relevant tax rules

---

## 🧪 Example Output


<img width="1920" height="1200" alt="Screenshot 2025-10-29 122056" src="https://github.com/user-attachments/assets/1bae7e4e-406e-4fa7-9ba4-e2355dbee197" />


<img width="608" height="425" alt="Screenshot 2025-10-29 122112" src="https://github.com/user-attachments/assets/29092b67-990a-40a4-9c1c-0fbcdf4aab10" />


---

## ✅ Key Features
- Context-grounded tax computation
- Slab-wise transparent calculation
- Policy-compliant deductions
- Consistent results for all users
- Enterprise-ready agent design

---

## 🔮 Future Enhancements
- Comparison between Old vs New tax regimes
- Integration with Form 16 / payroll data
- Tax-saving investment suggestions (policy-bound)
- Exportable tax computation report (PDF)

---

## 🏁 Conclusion
This project demonstrates the use of **UiPath Agents with context grounding** to build a **reliable, explainable, and compliant income tax advisory system**.

By grounding the AI strictly in official tax policy data, the solution avoids hallucinations and ensures trustworthiness—an essential requirement for financial and regulatory domains.

---

📌 *Built using UiPath Studio Web*

