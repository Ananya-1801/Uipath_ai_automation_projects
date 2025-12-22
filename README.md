# AI Automation & Agent-Based Projects

This repository contains a curated collection of **AI-assisted automation and agent-based workflows** developed **exclusively using UiPath Studio Web**.

The projects demonstrate **decision-driven automation**, **prompt-based agents**, and **practical RPA workflows**, built using UiPath’s cloud ecosystem and designed around real-world use cases.

---

## 📌 Repository Objective

The purpose of this repository is to showcase:

- End-to-end **AI-assisted RPA solutions**
- Agent-based and prompt-driven workflow design
- Practical automation using **UiPath Studio Web**
- Structured data handling using **JSON**
- Clean, modular, and scalable automation logic

---

## 🤖 Automation & Agent Projects

All projects listed below are developed using **UiPath Studio Web** and executed via **UiPath Orchestrator**.

---

### 1️⃣ Income Tax Calculator Agent
**Description:**  
An automation agent that computes income tax based on user-provided financial inputs and predefined tax slab rules.

**Highlights:**
- Rule-based tax computation  
- Input validation and boundary handling  
- JSON-based data exchange  

**Outcome:**  
Reduces manual calculation errors and demonstrates structured conditional logic.

---

### 2️⃣ Airline Compensation Agent
**Description:**  
An automation workflow that evaluates airline delay or cancellation scenarios to determine compensation eligibility.

**Highlights:**
- Policy-based rule evaluation  
- Scenario-driven decision logic  
- JSON input/output handling  

**Outcome:**  
Showcases real-world customer service automation and decision-centric workflows.

---

### 3️⃣ Stock Advisor Agent
**Description:**  
A **prompt-driven AI agent** that analyzes provided stock data and produces a **Buy / Don’t Buy** recommendation.

**Highlights:**
- Prompt-based analysis (no stored context)  
- Objective, data-driven recommendations  
- Mandatory financial disclaimer handling  
- JSON-based structured inputs  

**Outcome:**  
Demonstrates effective prompt engineering and ethical AI usage in financial scenarios.

---

### 4️⃣ Summarizing Text Agent
**Description:**  
A **simple AI-assisted RPA workflow** that generates concise summaries from unstructured text.

**Highlights:**
- Lightweight and stateless execution  
- Uses basic automation and AI tools  
- No context grounding or persistent memory  
- JSON-based input/output  

**Outcome:**  
Highlights clarity and simplicity in intelligent automation design.

---

### 5️⃣ Detect Language and Translate Agent
**Description:**  
An AI-assisted RPA workflow that detects the source language of input text and translates it into a target language.

**Highlights:**
- Automatic language detection  
- Translation workflow execution  
- Handles unstructured text input  
- JSON-based structured output  

**Outcome:**  
Demonstrates multilingual text processing within an RPA-first automation framework.

---

## 🧩 UiPath Platform Components Used

- **UiPath Studio Web** – Workflow and agent development  
- **UiPath Orchestrator** – Execution and monitoring  
- **UiPath Tenant Services** – Resource and environment management  
- **JSON** – Structured data exchange  

> Note:  
> Advanced components such as **Indexes** and **Storage Buckets** are not used across all agents and are applied only where appropriate. Several agents are intentionally designed to be **prompt-driven and stateless**.

---

## 🛠️ Technology Stack

- UiPath Studio Web  
- UiPath Orchestrator  
- JSON  
- Git & GitHub  

---

## 📂 Repository Structure

```text
ai-automation-agents/
│
├── Income-Tax-Calculator-Agent/
│   ├── README.md
│   └── *.uis
│
├── Airline-Compensation-Agent/
│   ├── README.md
│   └── *.uis
│
├── Stock-Advisor-Agent/
│   ├── README.md
│   └── *.uis
│
├── Summarizing-Text-Agent/
│   ├── README.md
│   └── *.uis
│
├── Detect-Language-and-Translate-Agent/
│   ├── README.md
│   └── *.uis
│
└── README.md
