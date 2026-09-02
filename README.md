# 🤖 Lead Intelligence Automation

An AI-powered lead qualification and urgency classification workflow built with **n8n, Google Gemini, Google Sheets, and Gmail**.

## 📌 Project Overview

This automation is designed to analyze incoming business leads and automatically determine their urgency level based on the lead's **budget and completion timeline**.

Instead of manually reviewing every inquiry, the workflow collects lead information through a form, uses an AI Agent powered by Google Gemini to classify the lead, stores the lead data in Google Sheets, and sends an email alert when a lead is classified as **High Urgency**.

## 🎯 Problem Statement

Businesses often receive multiple leads through inquiry forms. Manually reviewing each lead and identifying which prospects require immediate attention can be time-consuming.

This workflow automates the initial lead qualification process and helps prioritize leads based on predefined business rules.

## 💡 Solution

The workflow automatically:

1. Collects lead information through an n8n form.
2. Sends the lead information to an AI Agent.
3. Uses Google Gemini to analyze the lead.
4. Classifies the lead as:

   * **High Urgency**
   * **Medium Urgency**
   * **Low Urgency**
5. Stores the lead information and urgency tag in Google Sheets.
6. Checks whether the lead is High Urgency.
7. Sends a Gmail alert for High Urgency leads.

## 🔄 Workflow Flowchart

![Lead Intelligence Automation](screenshots/lead-intelligence-automation-flowchart.png)

## 🧠 Lead Classification Logic

The AI Agent follows these classification rules:

### 🔴 High Urgency

* High budget
* Urgent timeline of less than 15 days

### 🟡 Medium Urgency

* Medium budget
* Timeline around 1 month

### 🟢 Low Urgency

* Any lead that does not match the High or Medium Urgency conditions

The AI Agent is instructed to return only the urgency label without additional explanation.

## 🛠️ Technologies Used

* **n8n** — Workflow automation
* **Google Gemini** — AI-powered lead classification
* **Google Sheets** — Lead data storage
* **Gmail** — High-priority lead notifications
* **n8n Form Trigger** — Lead data collection

## 🚀 Example Use Case

A company receives a new inquiry from a potential customer who has:

```text
Name: John Smith
Company: Example Corp
Budget: High
Timeline: 10 Days
```

The AI Agent evaluates the lead and assigns:

```text
High Urgency
```

The lead is then stored in Google Sheets and an email alert is automatically sent so the sales team can respond quickly.

## 📈 Business Benefits

* Faster lead qualification
* Automated lead prioritization
* Reduced manual review
* Centralized lead tracking
* Immediate alerts for high-priority prospects
* Better sales response time

## 🔮 Future Improvements

Possible future enhancements include:

* Automatic CRM integration
* Lead scoring system
* Slack/Teams notifications
* Automatic sales representative assignment
* Follow-up email automation
* More advanced AI-based lead scoring
* Dashboard for lead analytics

## 👨‍💻 Author

**Faheem Abbas**

AI Automation | n8n | AI Workflows | Business Process Automation

#n8n #AIAutomation #GoogleGemini #LeadGeneration #LeadQualification #WorkflowAutomation #Automation #ArtificialIntelligence #bluemoonways
