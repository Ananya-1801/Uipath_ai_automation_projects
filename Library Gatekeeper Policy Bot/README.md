
# 📚 Library Gatekeeper Policy Bot

**SnowBot: The Agentic AI Winter Challenge 2025**

---
## 🚀 Project Overview

University libraries enforce strict and varying borrowing rules depending on **student type** (UG, PG, PhD) and **book category** (Reference, General, Reserved). Explaining these rules—especially when students make emotional or urgent pleas—often consumes significant staff time and leads to inconsistent decisions.

This project implements a **policy-grounded, agentic AI solution** using **UiPath Studio Web** that:

* Ingests official library policies
* Evaluates student profiles and book requests
* Makes **deterministic, explainable decisions**
* Resists emotional manipulation
* Produces firm, policy-backed responses without hallucination

This solution was built specifically for the **SnowBot: The Agentic AI Winter Challenge 2025**.

---

## 🎯 The Challenge

> *“Build an agent that ingests the Library Policy Manual and a Student Profile. Logically determine if a specific book request is allowed, even when the student includes emotional pleas or urgent excuses.”*

### Core Requirements

* Policy-grounded decision making
* Context-aware reasoning
* No hallucinated rules or exceptions
* Clear, firm, and explainable responses

---

## 🧠 Solution Approach

This agent follows a **policy-first reasoning architecture**, ensuring every decision is traceable back to documented library rules.

### Key Principles

* **Context Grounding**: The agent reasons only over retrieved policy data
* **Emotion-Aware, Not Emotion-Driven**: Emotional language is interpreted but never overrides policy
* **Deterministic Logic**: Identical inputs always produce identical outputs

---

## 🏗️ Architecture Overview

### Built With

* **UiPath Studio Web**
* **Storage Buckets** – for storing policy documents
* **Indexes** – for efficient policy retrieval
* **Agentic Workflows** – for structured decision logic

### High-Level Flow

1. Student submits a borrowing request
2. Agent retrieves:

   * Relevant policy clauses
   * Student profile details
3. Request is evaluated against policy constraints
4. A policy-grounded decision is generated
5. A firm, explainable response is returned

---

## 📥 Inputs

### 1. Library Policy Manual

Stored and indexed using UiPath Storage Buckets.
Defines:

* Borrowing limits by student type (UG / PG / PhD)
* Restrictions by book category:

  * **Reference**
  * **General**
  * **Reserved**

---

### 2. Student Profile

Includes:

* Student category (UG / PG / PhD)
* Enrollment status
* (Optional) borrowing history

---

### 3. Student Request

May contain:

* Book category ( mandatory ) 
* Requested duration ( mandatory ) 
* Emotional or urgent language (in student message which is optional )
  *(e.g., “I urgently need this for my thesis”)*

---

## 🧮 Decision Logic

The agent evaluates requests using the following steps:

1. Identify student type
2. Identify book category
3. Check requested borrowing duration
4. Retrieve relevant policy rules
5. Validate request against policy
6. Generate a decision:

   * ✅ Allowed
   * ❌ Not Allowed

Every step is grounded in retrieved policy context.

---

## 🧪 Example Scenario

### Student Request

> “I’m a PhD student and urgently need this Reference book for two weeks. It’s critical for my research.”

### Policy Evaluation

* Student Type: **PhD**
* Book Category: **Reference**
* Policy Rule: *Reference books are in-library use only*

### Final Decision

❌ Borrowing not allowed

---

## 📤 Example Output

> **Request Denied – Policy Restriction**
>
> According to the Library Policy Manual, *Reference* books are restricted to **in-library use only**, regardless of student category or urgency.
>
> You may access this book within the library premises or request assistance in locating a similar *General* category book eligible for checkout.

---

## 🖼️ Screenshots

<img width="1919" height="996" alt="image" src="https://github.com/user-attachments/assets/eeaa3500-21fe-4bf8-98ec-be323786b7be" />


### 🔹 Agent Workflow in UiPath Studio Web

<img width="1911" height="1005" alt="image" src="https://github.com/user-attachments/assets/731873c7-3e85-49d8-a078-b7c38a0c54a1" />

<img width="1916" height="1002" alt="image" src="https://github.com/user-attachments/assets/60d8c8e5-a2d1-4fc8-9360-a3985c49233b" />


### 🔹 Sample Agent Output

<img width="1919" height="1002" alt="image" src="https://github.com/user-attachments/assets/5d8af8f0-c842-4f34-a868-046faa0a097d" />

<img width="1035" height="551" alt="image" src="https://github.com/user-attachments/assets/2119364b-a879-4a5d-aa5a-e5149ca7e3b2" />


---

## 🛡️ Anti-Hallucination Safeguards

* The agent **cannot invent rules**
* All decisions are based on retrieved policy text
* No free-form reasoning without context grounding
* Emotional language does not alter outcomes

This ensures **consistent, auditable, and trustworthy behavior**.

---

## 🌟 Key Highlights

- ✅ Fully policy-grounded agent  
- ✅ Built entirely in UiPath Studio Web  
- ✅ Emotion-resilient decision making  
- ✅ Clear, explainable responses  
- ✅ Real-world institutional applicability  

---

## 🔗 Project Reference

UiPath Solution File:
[https://cloud.uipath.com/kiitejohagw/studio_/designer/8b044ada-9000-4479-82a9-16915a02916e?solutionId=b71f0899-cbf5-49ab-ca65-08de3e498e30](https://cloud.uipath.com/kiitejohagw/studio_/designer/8b044ada-9000-4479-82a9-16915a02916e?solutionId=b71f0899-cbf5-49ab-ca65-08de3e498e30)

---

## 🏁 Conclusion

This project demonstrates how **agentic AI**, when combined with **strong context grounding and deterministic logic**, can solve real-world policy enforcement challenges without hallucination or inconsistency.

It serves as a practical blueprint for deploying trustworthy AI agents in institutional environments.

---
## 🤝 Contributions

This project was developed as part of the **SnowBot: The Agentic AI Winter Challenge 2025**.

Contributions, suggestions, and improvements are welcome.  
If you would like to contribute:
1. Fork the repository
2. Create a feature branch
3. Commit your changes with clear descriptions
4. Open a pull request

All contributions should remain **policy-grounded** and must not introduce
hallucinated logic or undocumented assumptions.

