# Stage 1 — Root & Health Check API

A simple FastAPI application that introduces basic API endpoints for verifying that the application is running and healthy.

## Overview

Stage 1 focuses on implementing two basic endpoints:

- A **root endpoint** to confirm that the API is reachable.
- A **health check endpoint** to report the application's current status.

This stage builds on the Hello World setup from Stage 0 and establishes a basic structure for monitoring API availability before adding more functionality.

## Tech Stack

- Python
- FastAPI
- Uvicorn

## Project Structure

```text
stage1/
├── main.py
├── requirements.txt
├── README.md
└── venv/              # Local only, not committed
```

## Setup

### 1. Create and activate the virtual environment

```bash
python -m venv venv
```

Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
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

## Endpoints

### `GET /`

The root endpoint confirms that the API is reachable.

Example response:

```json
{
  "message": "API is running"
}
```

### `GET /health`

The health check endpoint reports the current health status of the application.

Example response:

```json
{
  "status": "healthy"
}
```

## Interactive API Documentation

FastAPI automatically generates interactive documentation:

- Swagger UI: `/docs`
- ReDoc: `/redoc`

For example:

```text
http://127.0.0.1:8000/docs
```

## Stage 1 Goal

The goal of this stage is to establish basic API availability and health-check endpoints that can be used to verify whether the FastAPI application is running correctly.

Further functionality will be introduced in subsequent stages.