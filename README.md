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

**REST API Foundation**
Build a clean and scalable CRUD API for creating, retrieving, updating, and deleting prompts.

⬇️

**Prompt Management**
Organize prompts using categories, tags, search, filtering, and persistent storage.

⬇️

**LLM Integration**
Execute and manage prompts across multiple LLM providers, enabling reusable prompt templates and model-specific configurations.

⬇️

**Prompt Intelligence**
Introduce prompt versioning, execution history, response tracking, and performance analytics to support iterative prompt engineering.

⬇️

**Production-Ready Backend**
Strengthen the API with authentication, testing, Docker, documentation, logging, monitoring, and deployment best practices.




---

## Status

🚧 Currently under active development.

This repository is part of my journey into backend engineering with Go, with a focus on building clean, maintainable APIs for AI-powered applications.

---

## Author

**Pralisha Tripathy**

Building AI systems, data engineering solutions, and backend infrastructure.
