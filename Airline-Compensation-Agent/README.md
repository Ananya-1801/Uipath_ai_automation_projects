
# ✈️ Airline Compensation Agent — UiPath RPA Project

## 📌 Overview

**Airline Compensation Agent** is an RPA workflow developed using **UiPath Studio Web** that automates the process of evaluating airline passengers’ eligibility for flight compensation based on a set of business rules. The automation takes user input, validates flight details against select criteria, and determines eligibility.

The solution incorporates multiple agents—including two specialized agents and a central Compensation Agent—as part of a complete RPA workflow. At the end of execution, users receive personalized email notifications with the results.

---

## 🚀 Key Features

* 🤖 **Automated Flight Eligibility Check**
  Processes user inputs to validate if passengers qualify for compensation based on defined parameters.

* 🧠 **Multi-Agent Processing**
  Utilizes two separate preprocessing agents along with a main **Compensation Agent** as modular components of the workflow.

* 📥 **Input Handling & Validation**
  Captures and validates user data before workflow execution.

* 📤 **Automated Email Output**
  Sends personalized email notifications with the final eligibility result to the user.

* 🛠️ **Built with UiPath Studio Web**
  Developed using modern UiPath cloud-native tooling and best practices, leveraging selectors, variables, arguments, and workflow modularization.

---

## 🧠 Workflow Description

The automation follows these general steps:

1. **Input Collection**

   * Accepts necessary flight and passenger details from UI or an input file.

2. **Pre-Processing Agents**

   * Two separate agents handle preliminary validation and data normalization.

3. **Compensation Evaluation**

   * Central Compensation Agent applies business logic to check eligibility.

4. **Outcome & Email Dispatch**

   * Generates a decision report and sends the output via email to the user.

The workflow is designed with modular, reusable components to improve maintainability and clarity, aligned with UiPath best practices for project structure and workflow design.([UiPath Documentation][1])


---

## 🛠️ Prerequisites

Before running the project, ensure:

* ✅ You have access to **UiPath Studio Web**.
* ✅ Email account/configuration settings are valid (SMTP or Orchestrator Assets if used).
* ✅ Required packages are installed and workflow dependencies are resolved.
* ✅ Input files are populated and available in the correct path.

---

## 🛠️ Tools & Technologies

- UiPath Studio Web  
- UiPath Orchestrator  
- JSON  

---

## 📈 Outcome

- Reduces manual policy evaluation effort  
- Demonstrates real-world customer service automation  
- Highlights decision-centric workflow design  

---

## 🎯 How to Run

1. Open **UiPath Studio Web**.
2. Clone or download this repository.
3. Navigate to the `Airline-Compensation-Agent` folder.
4. Open using Studio
5. Review and update input parameters (if needed).
6. Click **Debug and Run**.
7. Monitor execution and check the **Output** folder for logs.
8. Check the inbox for the result email ( ensure to use correct email in connection )

---

## 📬 Email Output

At the end of the workflow, users receive an email that includes:

* Flight details
* Evaluation result (Eligible / Not Eligible)
* Reasoning and next steps (if any)

> Emails are generated using templated logic and can be customized. 

---

## 🧩 Customization

You can extend the solution by:

* Adding support for additional airline policies.
* Integrating with airline APIs or databases for real-time validation.
* Using UiPath Orchestrator for scheduling or asset management.

---

## 📚 Best Practices Applied

This project follows common RPA and UiPath design principles such as:

* Modular workflow components for reusability and maintainability.
* Clear naming conventions for variables and workflows.
* Organized folder structure for inputs, outputs, and templates.
* Email notification integration for end-to-end automation.

---

## 👥 Contributing

Contributions are welcome! You can:

* Open issues for bugs or feature requests.
* Submit pull requests to improve workflows or documentation.




