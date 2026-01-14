---
name: Basecamp2 API
description: Use when working with basecamp2 api, cluster hdr, cluster lines, comments, embeddings, health check, people, projects, seed, todolist, todos, todos events, todos investigation, todos metrics, todos sessions, todos summary, topics, or making API calls to https://basecamp2.augur-api.com.
version: 1.0.5
---

# Basecamp2

Service-specific knowledge for basecamp2 microservice.

## API Documentation

- [OpenAPI Specification](https://basecamp2.augur-api.com/openapi.json)
- [Postman Collection](https://basecamp2.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### comments

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /comments/{id} | Get Comment by ID | [comments.md](comments.md#get-commentsid) |
| GET | /comments | List Comments | [comments.md](comments.md#get-comments) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### people

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /people/{id} | Get Person by ID | [people.md](people.md#get-peopleid) |
| GET | /people | List People with filters | [people.md](people.md#get-people) |
| GET | /people/{personId}/projects/{projectId}/todos | List Todos for Person on Project | [people.md](people.md#get-peoplepersonIdprojectsprojectIdtodos) |
| GET | /people/{id}/todos | List Todos for Person | [people.md](people.md#get-peopleidtodos) |

### projects

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /projects/{id} | Get Project by ID | [projects.md](projects.md#get-projectsid) |
| GET | /projects | List Projects | [projects.md](projects.md#get-projects) |
| GET | /projects/{projectId}/todolists/{todolistId}/todos | List Todos in Todolist within Project | [projects.md](projects.md#get-projectsprojectIdtodoliststodolistIdtodos) |
| GET | /projects/{id}/todolists | List Todolists for Project | [projects.md](projects.md#get-projectsidtodolists) |
| GET | /projects/{id}/todos | List Todos for Project | [projects.md](projects.md#get-projectsidtodos) |

### todolist

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /todolists/{id} | Get Todolist Details | [todolist.md](todolist.md#get-todolistsid) |
| GET | /todolists | List Todolists | [todolist.md](todolist.md#get-todolists) |

### todos

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /todos/{id}/comments | List Comments for Todo | [todos.md](todos.md#get-todosidcomments) |
| GET | /todos/{id} | Get Todo Details | [todos.md](todos.md#get-todosid) |
| GET | /todos | List Todos | [todos.md](todos.md#get-todos) |

### todos_events

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /todos/{id}/events | List Events for a Todo | [todos_events.md](todos_events.md#get-todosidevents) |
| GET | /todos/{id}/events/{eventNum} | Get Todo Event Details | [todos_events.md](todos_events.md#get-todosideventseventNum) |
| GET | /events | List Todo Events | [todos_events.md](todos_events.md#get-events) |

### todos_metrics

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /people/{id}/metrics | List Todo Metrics by Person | [todos_metrics.md](todos_metrics.md#get-peopleidmetrics) |
| GET | /projects/{id}/metrics | List Todo Metrics by Project | [todos_metrics.md](todos_metrics.md#get-projectsidmetrics) |
| GET | /todos/{id}/metrics | Get Todo Metrics Detail | [todos_metrics.md](todos_metrics.md#get-todosidmetrics) |
| GET | /metrics | List Todo Metrics | [todos_metrics.md](todos_metrics.md#get-metrics) |

### todos_sessions

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /todos/{id}/sessions | List Sessions for Todo | [todos_sessions.md](todos_sessions.md#get-todosidsessions) |
| POST | /todos/{id}/sessions | Create Session for Todo | [todos_sessions.md](todos_sessions.md#post-todosidsessions) |
| GET | /todos/{id}/sessions/{sessionId} | Get Session Details | [todos_sessions.md](todos_sessions.md#get-todosidsessionssessionId) |
| PUT | /todos/{id}/sessions/{sessionId} | Update Session | [todos_sessions.md](todos_sessions.md#put-todosidsessionssessionId) |
| DELETE | /todos/{id}/sessions/{sessionId} | Delete Session | [todos_sessions.md](todos_sessions.md#delete-todosidsessionssessionId) |

### todos_summary

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /todos-summary/{id} | Get Todo Summary Details | [todos_summary.md](todos_summary.md#get-todos-summaryid) |
| GET | /todos-summary | List Todo Summaries | [todos_summary.md](todos_summary.md#get-todos-summary) |
