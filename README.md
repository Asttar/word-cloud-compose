# Word Cloud

A microservice-based application for processing large text files and generating word frequency statistics. Users can upload text files, track processing status, retrieve word counts, and generate a word cloud.

## Requirements

Before running the application, ensure the following software is installed:

- Git
- Docker Desktop (includes Docker Compose)

No additional dependencies are required. All services are built and run inside Docker containers.

## Technologies

- React
- Spring Boot
- RabbitMQ
- PostgreSQL
- Flyway
- Docker
- Docker Compose
- Gradle

## Repositories

- `word-cloud-compose` – Docker Compose configuration for the application.
- `word-cloud-frontend` – React frontend.
- `word-cloud-core` – Spring Boot REST API.
- `word-cloud-worker` – Spring Boot worker service.

## Setup

Clone the repositories into a common parent directory using these folder names:

```bash
git clone https://github.com/Asttar/word-cloud-compose.git compose
git clone https://github.com/Asttar/word-cloud-frontend.git frontend
git clone https://github.com/Asttar/word-cloud-core.git core
git clone https://github.com/Asttar/word-cloud-worker.git worker
```

```text
word-cloud/
├── compose/
├── frontend/
├── core/
└── worker/
```

Then run:

```bash
cd compose
docker compose up --build
```

## Access

- Frontend: http://localhost:5173
- RabbitMQ Management: http://localhost:15672
  - Username: `guest`
  - Password: `guest`
