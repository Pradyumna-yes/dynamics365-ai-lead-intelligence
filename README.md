# 🚀 AI Sales Assistant (Power Automate + Dynamics 365)

## 📌 Overview

This project automates lead qualification using AI.

It analyzes lead data (company, topic, job title) and generates:

* 🔢 AI Score
* 💡 Insight
* 🎯 Next Best Action

---

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

https://github.com/user-attachments/assets/d124814c-0ab1-4875-808d-63b571b14607

<img width="1691" height="952" alt="User Trigger" src="https://github.com/user-attachments/assets/d124814c-0ab1-4875-808d-63b571b14607" />

---

### 2️⃣ Get Lead Data

Fetches Company Name, Topic, and Job Title

https://github.com/user-attachments/assets/fd6999c2-8437-4656-b6b8-b171e083ff41

<img width="578" height="300" alt="Get Lead Data" src="https://github.com/user-attachments/assets/fd6999c2-8437-4656-b6b8-b171e083ff41" />

---

### 3️⃣ Format Prompt

Transforms lead data into structured input for AI

---

### 4️⃣ Call AI API

Sends request to DeepSeek model

https://github.com/user-attachments/assets/d959c1ac-0fc2-49d0-9e93-1643fb89fa78

<img width="578" height="885" alt="Call AI API" src="https://github.com/user-attachments/assets/d959c1ac-0fc2-49d0-9e93-1643fb89fa78" />

---

### 5️⃣ Parse JSON Response

Extracts structured AI output (score, action, urgency, reason)

---

### 6️⃣ Update Lead Fields

Updates AI Score, Insight, and Next Best Action

https://github.com/user-attachments/assets/fd9367a4-3b72-4cd2-b231-8323655e0680

<img width="1680" height="328" alt="Update Lead Fields" src="https://github.com/user-attachments/assets/fd9367a4-3b72-4cd2-b231-8323655e0680" />

---

### 7️⃣ Create Task in CRM

Creates a follow-up task linked to the Lead

https://github.com/user-attachments/assets/403b5e62-e34e-453c-977a-ba1843bce77e

<img width="1681" height="935" alt="Create Task" src="https://github.com/user-attachments/assets/403b5e62-e34e-453c-977a-ba1843bce77e" />


---

## 🔥 Features

* AI-based lead scoring
* Automated CRM updates
* Smart task creation
* Structured prompt engineering
* Real-time decision support

---

## 📸 Screenshots
# 🚀 AI Sales Assistant (Power Automate + Dynamics 365)

## 📌 Overview

This project automates lead qualification using AI.

It analyzes lead data (company, topic, job title) and generates:

* 🔢 AI Score
* 💡 Insight
* 🎯 Next Best Action

---

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

---

## 🔥 Features

* AI-based lead scoring
* Automated CRM updates
* Smart task creation
* Structured prompt engineering
* Real-time decision support

---

## 📸 Screenshots

## 🔄 End-to-End Process Flow

### 🧠 How the AI Sales Assistant Works

1. **User triggers the flow**

   * From a Lead record in Dynamics 365
   * Using a manual button ("Run Flow")

2. **Fetch Lead Data**

   * System retrieves:

     * Company Name
     * Topic / Description
     * Job Title

3. **Prepare AI Input**

   * Data is structured into a prompt using Power Automate
   * Example:

     ```
     Company: XYZ Corp
     Topic: CRM implementation
     Job Title: Sales Director
     ```

4. **Call AI Model (DeepSeek API)**

   * HTTP request is sent with prompt
   * AI analyzes lead quality and intent

5. **AI Response (Structured JSON)**

   * The model returns:

     * `score` (0–10)
     * `action` (call/email/wait/discard)
     * `urgency` (low/medium/high)
     * `reason` (explanation)

6. **Parse AI Response**

   * Power Automate extracts values using Parse JSON

7. **Update Lead in Dynamics 365**

   * AI Score → saved to custom field
   * AI Insight → explanation stored
   * Next Best Action → recommendation

8. **Create Follow-up Task**

   * Automatically creates a task
   * Linked to the Lead
   * Example:

     * Subject: "Follow up: call"
     * Description: AI-generated insight

---

### 🔁 Visual Flow (Simplified)
## 🔁 Visual Flow (Simplified)

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

Your Name



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

Your Name
