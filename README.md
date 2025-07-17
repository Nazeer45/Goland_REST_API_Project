# Students API

A Representational State Transfer (RESTful) API project for managing student records, built with Go and SQLite to simulate real-world backend systems used in microservices architectures, enabling consistent and secure data exchange for client-facing applications.

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

# Install dependencies
go get -u github.com/ilyakaznacheev/cleanenv
go get github.com/go-playground/validator/v10
go get github.com/mattn/go-sqlite3

# Run the server
go run .\cmd\students-api\main.go -config config/local.yaml
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
