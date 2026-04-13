# 🚀 AI Sales Assistant (Power Automate + Dynamics 365)

## 📌 Project Description

This project demonstrates an AI-powered lead qualification system built using **Microsoft Dynamics 365**, **Power Automate**, and an external **LLM (DeepSeek API)**.

The solution analyzes lead information such as company, topic, and job title to generate:

* 🔢 AI-based lead score
* 💡 Contextual insight
* 🎯 Recommended next best action

All outputs are automatically written back into Dynamics 365 and used to trigger follow-up actions like task creation.

---

## 🎯 Why I Built This

In traditional CRM workflows, lead qualification is:

* Manual
* Time-consuming
* Inconsistent across sales teams

This project explores how **LLMs can augment CRM systems** by:

* Automating decision-making
* Standardizing lead evaluation
* Reducing response time
* Assisting sales teams with actionable insights

---

## 🧪 Project Scope (POC)

This is a **Proof of Concept (POC)** built to understand:

* How to integrate **LLMs with Dynamics 365**
* How to structure prompts for business decision-making
* How to orchestrate AI workflows using **Power Automate**
* How to handle structured AI responses (JSON) inside enterprise systems

---

## 🚀 Exploration Phase

This project represents the **first phase** of exploring LLM integration within enterprise CRM systems.

Future iterations may include:

* Automated triggers (real-time scoring)
* Email/communication automation
* Multi-model AI support
* Analytics and reporting dashboards

---

## 🧠 Key Learning

This project helped in understanding:

* End-to-end AI workflow integration
* Prompt engineering for business use cases
* Dataverse + Power Automate orchestration
* Practical challenges in connecting LLMs with enterprise systems


## 🧠 How It Works

1. User selects a Lead in Dynamics 365
2. Flow is triggered manually
3. Lead data is fetched
4. Sent to DeepSeek API
5. AI returns:

   * score
   * action
   * urgency
   * reason
6. CRM is updated automatically
7. Task is created for follow-up

---

## ⚙️ Tech Stack

* Microsoft Power Automate
* Dynamics 365 (Dataverse)
* DeepSeek API (LLM)
* JSON Parsing

<img width="1024" height="1536" alt="System Design" src="https://github.com/user-attachments/assets/f4f0da01-0159-4b4d-a989-33ab7f01fa78" />


  ## 🔁 Visual Flow

---

### 1️⃣ User Trigger

User manually runs the flow from a Lead record in Dynamics 365

<img width="1691" height="952" alt="User Trigger" src="https://github.com/user-attachments/assets/d124814c-0ab1-4875-808d-63b571b14607" />

---

### 2️⃣ Get Lead Data

Fetches Company Name, Topic, and Job Title

<img width="578" height="300" alt="Get Lead Data" src="https://github.com/user-attachments/assets/fd6999c2-8437-4656-b6b8-b171e083ff41" />

---

### 3️⃣ Format Prompt

Transforms lead data into structured input for AI

---

### 4️⃣ Call AI API

Sends request to DeepSeek model

<img width="578" height="885" alt="Call AI API" src="https://github.com/user-attachments/assets/d959c1ac-0fc2-49d0-9e93-1643fb89fa78" />

---

### 5️⃣ Parse JSON Response

Extracts structured AI output (score, action, urgency, reason)

---

### 6️⃣ Update Lead Fields

Updates AI Score, Insight, and Next Best Action

<img width="1680" height="328" alt="Update Lead Fields" src="https://github.com/user-attachments/assets/fd9367a4-3b72-4cd2-b231-8323655e0680" />

---

### 7️⃣ Create Task in CRM

Creates a follow-up task linked to the Lead

<img width="1681" height="935" alt="Create Task" src="https://github.com/user-attachments/assets/403b5e62-e34e-453c-977a-ba1843bce77e" />


---

## 🔥 Features

* AI-based lead scoring
* Automated CRM updates
* Smart task creation
* Structured prompt engineering
* Real-time decision support

---


## 📦 Setup

1. Import the flow ZIP into Power Automate
2. Configure API key
3. Connect Dataverse
4. Run from a Lead record

---

## 🚀 Future Improvements

* Auto-trigger on lead update
* Email automation
* Dashboard analytics
* Multi-model AI support

---

## 👨‍💻 Author

Prady 


