# Students API

A RESTful API for managing student records, built with Go.

## Features

- 🚀 Fast and lightweight Go server
- 🗄️ SQLite database for persistent storage
- 🔒 Input validation and error handling
- 📋 CRUD endpoints for students
- ⚙️ Configurable via YAML and environment variables
- 📑 Structured logging with slog
- 🛑 Graceful shutdown

## Endpoints

| Method | Endpoint                | Description                |
|--------|------------------------|----------------------------|
| POST   | `/api/students`        | Create a new student       |
| GET    | `/api/students/{id}`   | Get student by ID          |
| GET    | `/api/students`        | List all students          |

## Getting Started

```bash
git clone https://github.com/yourusername/students-api.git
cd students-api
go run ./cmd/students-api
```

## Configuration

Edit `config.yaml` to set environment, address, and database path.

## Project Structure

```
cmd/students-api/           # Main entry point
internal/config/            # Configuration loader
internal/http/handlers/     # HTTP handlers
internal/storage/sqlite/    # SQLite storage implementation
```

## Logging

Uses Go's `slog` for structured logs.

##
