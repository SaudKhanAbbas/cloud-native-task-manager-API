# Cloud-Native Task Manager API

A production-ready REST API for task management built with **Node.js**, **Express**, **PostgreSQL**, and **Prisma**. The project includes JWT authentication, Docker support, CI/CD, and cloud deployment assets.

## Tech Stack

* Node.js
* Express.js
* PostgreSQL
* Prisma ORM
* JWT Authentication
* Docker & Docker Compose
* AWS EC
* Terraform
* Kubernetes
* GitHub Actions

## Features

* User authentication with JWT
* Task CRUD operations
* Search, filtering, sorting, and pagination
* Request validation
* Centralized error handling
* Health check endpoints
* Swagger API documentation
* Dockerized development environment
* AWS deployment configuration

## Project Structure

```text
src/
├── config/
├── controllers/
├── middleware/
├── routes/
├── services/
├── utils/
├── validators/

prisma/
tests/
terraform/
k8s/
nginx/
```

## Getting Started

1. Clone the repository.

2. Install dependencies:

```bash
npm install
```

3. Create an environment file:

```bash
cp .env.example .env
```

4. Generate Prisma Client and run migrations:

```bash
npm run prisma:generate
npm run prisma:migrate
```

5. Start the development server:

```bash
npm run dev
```

The API will be available at:

```text
http://localhost:3000
```

Swagger Documentation:

```text
http://localhost:3000/api-docs
```

## Useful Commands

```bash
npm run dev
npm start
npm test
npm run lint
npm run prisma:generate
npm run prisma:migrate
```

## Docker

Start the application with Docker:

```bash
docker compose up --build
```

## API Endpoints

### Authentication

* `POST /api/v1/auth/register`
* `POST /api/v1/auth/login`

### Tasks

* `GET /api/v1/tasks`
* `POST /api/v1/tasks`
* `GET /api/v1/tasks/:taskId`
* `PATCH /api/v1/tasks/:taskId`
* `DELETE /api/v1/tasks/:taskId`

### Health

* `GET /api/v1/health`
* `GET /api/v1/health/live`
* `GET /api/v1/health/ready`

## License

This project is intended for learning and portfolio purposes.

This version removes repetitive sections while keeping the important information recruiters or contributors typically look for. It also makes the README easier to scan on GitHub.
