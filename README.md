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

```
User Trigger
     ↓
<img width="1691" height="952" alt="image" src="https://github.com/user-attachments/assets/d124814c-0ab1-4875-808d-63b571b14607" />
Get Lead Data
     ↓
<img width="578" height="300" alt="image" src="https://github.com/user-attachments/assets/fd6999c2-8437-4656-b6b8-b171e083ff41" />
Format Prompt
     ↓
Call AI API
     ↓
<img width="578" height="885" alt="image" src="https://github.com/user-attachments/assets/d959c1ac-0fc2-49d0-9e93-1643fb89fa78" />

Parse JSON Response
     ↓
Update Lead Fields
     ↓
<img width="1680" height="328" alt="image" src="https://github.com/user-attachments/assets/fd9367a4-3b72-4cd2-b231-8323655e0680" />
Create Task in CRM
<img width="1681" height="935" alt="image" src="https://github.com/user-attachments/assets/403b5e62-e34e-453c-977a-ba1843bce77e" />

```

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
