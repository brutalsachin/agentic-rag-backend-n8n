# 🚀 Agentic RAG Backend using n8n

A production-style Agentic Retrieval-Augmented Generation (RAG) backend built using **n8n + OpenAI**.

This system supports:
- Stateful multi-session memory
- Vector-based knowledge retrieval
- Step-controlled agent reasoning loop
- Webhook-based REST API endpoint

---

## 📌 Overview

This project implements an autonomous AI backend capable of:

1. Accepting user queries via Webhook API
2. Maintaining session-based conversational memory
3. Retrieving relevant documents from a Vector Store
4. Running an agent loop for controlled reasoning
5. Returning structured JSON responses

---

## 🏗 Architecture

### 🔄 Flow Diagram

<img width="1570" height="723" alt="image" src="https://github.com/user-attachments/assets/fb89c829-c948-42b4-be7b-adc08b90b569" />





---

## 🧠 Key Features

- ✅ Webhook API endpoint
- ✅ Session-based chat memory
- ✅ Retrieval-Augmented Generation (RAG)
- ✅ Step-controlled agent loop
- ✅ Vector search integration
- ✅ Structured JSON response format

---

## 🔍 How RAG Works in This System

1. User query is embedded
2. Vector search retrieves relevant chunks
3. Retrieved context is injected into the LLM
4. LLM generates grounded response
5. Memory stores conversation state

---

## 🛠 Tech Stack

- **n8n** – Workflow orchestration
- **OpenAI** – Chat model
- **Vector Store** – Knowledge retrieval
- **REST Webhook API**
- **Session-based Memory**

---

## 📦 Example API Request

```json
POST /webhook-test/agent-webhook

{
  "sessionId": "user123",
  "query": "What is ai?"
}
