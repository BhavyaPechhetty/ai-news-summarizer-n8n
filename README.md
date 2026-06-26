# AI News Summarizer using n8n

## 📌 Overview

This project is an automated AI News Summarizer built using **n8n**, **Google Gemini AI**, **RSS feeds**, and **Gmail**. It automatically collects the latest AI news, summarizes the articles using Gemini AI, and delivers a formatted email to the user.



## 🚀 Features

* Automated execution using Schedule Trigger
* Fetches AI news from multiple RSS feeds
* Merges and limits articles before processing
* Summarizes news using Google Gemini 3.1 Flash Lite
* Sends daily email summaries through Gmail
* Fully automated workflow built using n8n



## 🛠️ Workflow

```text
Schedule Trigger
      ↓
RSS Feed
      ↓
Merge
      ↓
Limit
      ↓
Data Aggregate
      ↓
Google Gemini AI
      ↓
Gmail
```



## 💻 Technologies Used

* n8n
* Google Gemini API
* Gmail API
* RSS Feeds
* Google Cloud Platform


## 📂 Repository Contents

* `NEWS-Summarizer new.json` – Exported n8n workflow
* `screenshots/` – Workflow and execution screenshots



## ⚙️ How to Use

1. Import the workflow into n8n.
2. Configure your Google Gemini API credentials.
3. Configure Gmail OAuth credentials.
4. Replace the placeholder recipient email with your own email address.
5. Execute the workflow manually or activate the Schedule Trigger.



## 📚 Learning Outcomes

* Workflow automation with n8n
* RSS feed integration
* AI-powered news summarization
* Google Gemini API integration
* Gmail OAuth authentication
* API debugging and workflow optimization

## ⚠️ Challenges Faced

During the development of this project, I encountered several challenges:

- Faced Gemini API quota limits (HTTP 429) and switched to a supported model with available free-tier quotas.
- Configured Google Gemini API credentials and generated a new API key.
- Connected the Google Gemini Chat Model correctly in n8n.
- Resolved OAuth authentication issues while integrating Gmail.
- Limited the number of RSS articles before summarization to optimize token usage and improve workflow performance.
- Tested and debugged the workflow node by node until the complete automation executed successfully.
---

## 👩‍💻 Author

**Bhavya Sree**
