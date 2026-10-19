# Flyrank FastAPI — Stage 0

A minimal **Hello World API** built with FastAPI as the starting stage of the project.

## Overview

Stage 0 focuses on setting up the basic FastAPI application and verifying that the development environment and API server are working correctly.

This stage intentionally contains only a simple endpoint. CRUD functionality and additional features will be implemented in later stages.

## Tech Stack

- Python
- FastAPI
- Uvicorn

## Project Structure

```text
stage0/
├── main.py
├── .gitignore
└── README.md
```

## Getting Started

### 1. Create and activate the virtual environment

```bash
python -m venv venv
```

On Windows:

```bash
venv\Scripts\activate
```

### 2. Install dependencies

```bash
pip install fastapi uvicorn
```

### 3. Run the application

```bash
uvicorn main:app --reload
```

The API will be available at:

```text
http://127.0.0.1:8000
```

## Endpoint

### `GET /`

Returns a simple Hello World response.

Example response:

```json
{
  "message": "Hello World"
}
```

## API Documentation

FastAPI automatically provides interactive API documentation:

- `/docs` — Swagger UI
- `/redoc` — ReDoc

For example:

```text
http://127.0.0.1:8000/docs
```

## Stage 0 Goal

The goal of this stage is to establish a working FastAPI application that can be run locally and accessed through a basic HTTP endpoint.

Future stages will build on this foundation with additional functionality.