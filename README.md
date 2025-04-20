# 🧠 RAG (Retrieval-Augmented Generation) with Spring AI, Ollama, and pgvector

A lightweight, local-first RAG application built with Spring Boot, Ollama, and PostgreSQL (pgvector). This project enables you to perform Retrieval-Augmented Generation using your own documents, running entirely on your machine without relying on external APIs.

## 🚀 Features

- **Local LLM Integration**: Utilizes [Ollama](https://ollama.ai/) to run large language models locally.
- **Vector Store**: Employs PostgreSQL with the `pgvector` extension for efficient vector storage and retrieval.
- **Document Processing**: Integrates Apache Tika for parsing and processing various document formats.
- **Spring AI Integration**: Leverages Spring AI's capabilities for seamless AI model integration.
- **RESTful API**: Provides a REST endpoint to interact with the RAG system.

## 🛠️ Tech Stack

- **Backend**: Spring Boot 3.4.4
- **AI Integration**: Spring AI 1.0.0-M7
- **Vector Store**: PostgreSQL with `pgvector`
- **LLM**: Ollama
- **Document Parsing**: Apache Tika

## 📦 Prerequisites

Ensure you have the following installed:

- **Java**: JDK 21
- **Maven**: For building the project
- **Docker**: For running PostgreSQL with `pgvector`
- **Ollama**: For local LLM inference

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/Shivam798/Rag.git
```
### 2. Run the Spring Boot Application
Navigate to the main application class:
```bash
src/main/java/com/example/AIRag/AiRagApplication.java
```

### 3. Use Postman to Send Chat Queries
```bash
http://localhost:8080/api/chat
```
Body (raw, text/plain): Enter the query you want to chat with pdf

### ⚠️Note: 
This application uses your local machine's resources to process requests using Ollama.
Response time may vary based on your system’s performance (CPU, memory, etc.).


