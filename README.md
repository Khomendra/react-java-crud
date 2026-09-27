# EMS: User & Employee Management System

A production-style full-stack learning project: **React + TypeScript**, **Java + Spring Boot + Spring Security**, **PostgreSQL**, **JWT**, thorough **testing**, and **Docker**.

> Status: Phase 1 (architecture and project skeleton). Sections marked *(coming)* get filled in as each phase lands.

## Overview

Admins manage employee accounts (create, update, delete, roles, images). Employees log in, manage their own profile and browse a limited company directory. The full design lives in [`docs/EMS-Project-Plan.docx`](docs/EMS-Project-Plan.docx).

## Tech stack

| Layer    | Tech |
|----------|------|
| Frontend | React 19, TypeScript, Vite, React Router, TanStack Query, Axios, React Hook Form + Zod, Tailwind CSS |
| Backend  | Java 25, Spring Boot 4.1, Spring Web, Spring Data JPA, Spring Security (JWT resource server), Bean Validation |
| Database | PostgreSQL 18, Flyway migrations |
| Cache    | Redis 8 (login rate limiting, logout token denylist, caching) |
| Testing  | JUnit 5, Mockito, MockMvc, Testcontainers, Vitest, React Testing Library, MSW, Postman + Newman |
| DevOps   | Docker, Docker Compose |

## Repository layout

```
react-java-crud/
├── backend/        Spring Boot API (Maven)
├── frontend/       React app (Vite)
├── database/       manual SQL: practice and inspection queries
├── postman/        API collection + environments
├── docs/           project plan and design notes
├── .env.example    all configuration variables (copy to .env)
└── README.md
```

## Prerequisites

| Tool | Version | Check |
|------|---------|-------|
| JDK | 25 (21 minimum) | `java -version` |
| Node.js | 24 LTS | `node -v` |
| Git | any recent | `git --version` |
| PostgreSQL | 18 | `psql --version` *(installed in Phase 2)* |
| Docker Desktop | recent | `docker --version` *(needed from Phase 3 for Redis and Testcontainers)* |
| Postman | recent | *(Phase 13)* |

Maven is **not** required: the backend ships with the Maven Wrapper (`mvnw`).

## Getting started *(coming)*

1. Copy `.env.example` to `.env` and fill in values.
2. Database setup (Phase 2)
3. Run backend (Phase 3)
4. Run frontend (Phase 10)

## Sections coming later

Architecture · Database schema · API documentation · Running tests · Postman · Docker · Future improvements
