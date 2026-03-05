## Introduction

This project demonstrates an automated AI workflow pipeline that integrates LLM reasoning, web search, data logging, and automated email delivery.

The workflow processes a user query, enriches it with web information, generates AI insights, stores results in Google Sheets, and sends the final output via email.

The system is designed as a modular AI automation pipeline, where each node performs a specific task such as model interaction, web search, data processing, or notification.


This type of workflow is useful for AI research assistants, automated reporting systems, knowledge retrieval tools, and decision-support applications.

---

![Workflow Architecture](https://github.com/Shrushtid13/n8N-email-generation/blob/main/Screenshot%202026-03-05%20111309.png)

---

## Tech Stack

- OpenAI API
- Tavily Search API
- Google Sheets API
- Gmail API
- REST APIs
- n8n

---

## Workflow Logic

1. **Trigger Workflow** – The workflow starts when the user clicks *Execute Workflow*.
2. **Initial LLM Processing** – The input query is sent to the language model for initial understanding and response generation.
3. **Edit Fields** – The generated data is formatted and structured for further processing.
4. **Update Google Sheets** – Intermediate data is stored in Google Sheets for logging and tracking.
5. **Web Search (Tavily API)** – An HTTP request is made to retrieve relevant web information.
6. **AI Agent Processing** – The AI agent uses the OpenAI chat model to analyze the query along with retrieved search results.
7. **Store Final Output** – The final response is updated in Google Sheets.
8. **Send Email Notification** – The generated result is sent to the user via Gmail.
