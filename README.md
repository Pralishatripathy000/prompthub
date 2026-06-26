# 🚀 PromptHub

> A production-ready REST API built in Go for managing, organizing, and versioning LLM prompts.

![Go](https://img.shields.io/badge/Go-1.24-00ADD8?logo=go)
![REST API](https://img.shields.io/badge/REST-API-blue)
![Status](https://img.shields.io/badge/Status-Building-orange)
![License](https://img.shields.io/badge/License-MIT-green)

---

## Why PromptHub?

As applications increasingly rely on Large Language Models, prompts become an important part of the software stack.

Yet most developers still store prompts inside source code, scattered text files, or notebooks, making them difficult to organize, version, search, and reuse.

PromptHub is an attempt to solve that problem through a lightweight REST API built entirely in Go.

The project is also a hands-on exploration of backend engineering fundamentals, including HTTP servers, REST APIs, JSON serialization, routing, request handling, and clean project architecture.

---

## Features

- Create prompts
- Retrieve prompts
- Update prompts
- Delete prompts
- Search prompts
- Organize by category
- Tag support
- Health Check endpoint

---

## Example Prompt

```json
{
    "id": 1,
    "title": "Meeting Summarizer",
    "prompt": "Summarize the following meeting transcript...",
    "category": "Productivity",
    "model": "GPT-4.1",
    "tags": [
        "summary",
        "meetings"
    ]
}
```

---

## API Endpoints

| Method | Endpoint | Description |
|---------|----------|-------------|
| GET | `/health` | Health check |
| GET | `/prompts` | Retrieve all prompts |
| GET | `/prompts/{id}` | Retrieve a prompt |
| POST | `/prompts` | Create a prompt |
| PUT | `/prompts/{id}` | Update a prompt |
| DELETE | `/prompts/{id}` | Delete a prompt |

---
## 🛠️ Tech Stack

### Backend
- Go
- Go Standard Library (`net/http`, `encoding/json`, `strconv`, `strings`)

### API
- REST Architecture
- JSON
- HTTP

### Development & Testing
- Postman
- Git
- GitHub Codespaces

---

## Project Structure

```text
prompthub/

├── cmd/
│   └── main.go
│
├── handlers/
│
├── models/
│
├── routes/
│
├── utils/
│
├── README.md
│
├── go.mod
│
└── .gitignore
```

---

## Learning Goals

This project is being built to understand:

- Go fundamentals
- REST API design
- HTTP request lifecycle
- JSON serialization
- Backend architecture
- Error handling
- Project organization
- Building production-style services

---

## 🗺️ Roadmap

**Prompt Management**
⬇️
**RESTful CRUD API** → Create, retrieve, update, and delete reusable LLM prompts
⬇️
**Prompt Organization** → Categories, tags, search, and filtering for efficient prompt discovery
⬇️
**Persistent Storage** → Store prompts securely using a database instead of in-memory storage
⬇️
**Authentication & Access Control** → User accounts, JWT authentication, and protected endpoints
⬇️
**LLM Integration** → Execute saved prompts directly against supported LLM providers and manage model-specific prompt configurations
⬇️
**Prompt Versioning & History** → Track prompt revisions, compare changes, and restore previous versions
⬇️
**Developer Experience** → API documentation, Postman collection, Docker support, and automated testing
⬇️
**Production-Ready Backend** → Logging, configuration management, deployment, monitoring, and scalable architecture


---

## Status

🚧 Currently under active development.

This repository is part of my journey into backend engineering with Go, with a focus on building clean, maintainable APIs for AI-powered applications.

---

## Author

**Pralisha Tripathy**

Building AI systems, data engineering solutions, and backend infrastructure.
