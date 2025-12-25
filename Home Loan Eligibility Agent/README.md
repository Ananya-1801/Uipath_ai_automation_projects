# 🏦 Corporate Home Loan Eligibility Agent (UiPath)

## 📌 Project Overview
The **Corporate Home Loan Eligibility Agent** is an AI-powered decisioning system built using **UiPath Studio Web**.  
It determines the **maximum home loan amount an employee is eligible for** by strictly grounding its decisions in **company-specific HR and financial policies**.

The agent ensures **accuracy, consistency, transparency, and policy compliance** across all eligibility decisions by using **context grounding via indexed policy documents**.

---

## 🎯 Objectives
- Determine employee home loan eligibility based on company rules
- Calculate the maximum eligible loan amount
- Ensure decisions are **policy-aligned and explainable**
- Prevent AI hallucinations using **context grounding**
- Provide consistent outcomes for all employees

---

## 🧠 Key Concept: Context Grounding
Context grounding restricts the AI agent to use **only approved internal documents** as its source of truth.

In this project:
- Company loan policies are stored in **Storage Buckets**
- Policies are indexed using **UiPath Indexes**
- The AI agent retrieves information **only from these indexes**
- Employee data is passed dynamically at runtime

This ensures:
- ❌ No invented rules  
- ❌ No external financial assumptions  
- ✅ Fully auditable decisions  

---
## 🏗️ Solution Architecture

Employee Input (Arguments / App)
↓
Policy Documents (Storage Bucket)
↓
Policy Index (Context Grounding)
↓
AI Eligibility Agent
↓
Loan Eligibility Decision + Explanation


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
- Prompt-based reasoning
- Policy-restricted decision making

---

## 📊 Datasets Used

### 1️⃣ Employee_Data.xlsx
Contains employee attributes used at runtime:
- Employee ID
- Grade
- Employment Type
- Monthly Salary
- Total Experience

> This data is **not indexed** and is passed as arguments to the agent.

---

### 2️⃣ Loan_Policy_Context.xlsx
Contains company policy data used for grounding:

#### Sheet: Loan_Policy_Rules
- Grade-based loan multipliers
- Maximum loan caps
- Minimum salary thresholds

#### Sheet: Eligibility_Rules
- Employment type eligibility
- Minimum experience rules
- EMI affordability limits

#### Sheet: Policy_Metadata
- Policy ID
- Version
- Effective date
- Issuing department

> This file is uploaded to a **Storage Bucket** and indexed for context grounding.

---

## 📚 Index Configuration

- **Index Name:** `home-loan-policy-index`
- **Source:** Loan_Policy_Context.xlsx
- **Purpose:** Provide authoritative policy context to the AI agent

Only policy files are indexed to prevent leakage of dynamic or sensitive data.

---

## 🤖 Agent Prompt Design

### 🔐 System Prompt
Defines strict guardrails to ensure:
- Only indexed policy data is used
- No assumptions or external knowledge are applied
- Every decision includes a policy-based explanation

### 🧑‍💼 User Prompt
Provides structured employee input at runtime and instructs the agent to:
- Evaluate eligibility
- Calculate loan amount
- Explain the decision using policy references

---

## 🧪 Example Output

**Eligibility Status:** Eligible

**Maximum Eligible Loan Amount:** $2,880,000

**Policy-Based Explanation:**

The employee is eligible for a home loan based on the following policy rules:

1. **Employment Type:** The employee is a permanent employee, which satisfies the eligibility condition as per the policy (RuleType: EmploymentType | RuleValue: Permanent | EligibilityStatus: Eligible).
2. **Minimum Experience:** The employee has 3 years of total experience, which exceeds the minimum requirement of 2 years (RuleType: MinExperienceYears | RuleValue: 2 | EligibilityStatus: Eligible).
3. **Grade and Loan Multiplier:** The employee's grade is "C," which corresponds to a loan multiplier of 40. The maximum loan amount for grade C is $8,000,000, and the minimum monthly salary required is $30,000. The employee's monthly salary is $6,000, which is below the minimum salary requirement for grade C. However, the loan amount is calculated as follows:
    - Loan Amount = Monthly Salary x Loan Multiplier = $6,000 x 40 = $2,880,000.
4. **EMI Cap:** The policy states that the EMI must not exceed 40% of the monthly salary. This condition is satisfied as the calculated loan amount is within the permissible limit.

**Policy Reference:**

- PolicyID: LP001
- PolicyName: Corporate Home Loan Policy
- Version: v3.2
- EffectiveDate: 2024-04-01
- IssuedBy: HR and Finance Department

<img width="1915" height="1003" alt="image" src="https://github.com/user-attachments/assets/ad846ba3-6b8a-4e84-b112-4d158cc6ece2" />


---

## ✅ Key Features
- Context-grounded AI decisioning
- Transparent and explainable outcomes
- Policy-driven and consistent logic
- Enterprise-ready architecture
- Easy to extend with approvals or audits

---

## 🔮 Future Enhancements
- HR approval workflow using Action Center
- EMI simulation and affordability scoring
- Integration with payroll systems
- Audit logs and compliance dashboards

---

## 🏁 Conclusion
This project demonstrates how **UiPath Agents with context grounding** can be used to build **reliable, explainable, and policy-compliant AI systems** for financial decision-making within enterprises.

The solution prioritizes **accuracy, governance, and transparency**, making it suitable for real-world corporate environments.

---

📌 *Built using UiPath Studio Web*
