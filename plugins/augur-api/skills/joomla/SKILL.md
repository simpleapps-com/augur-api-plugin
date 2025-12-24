---
name: Joomla API
description: Use when working with categories, content, contentitem tag map, extensions, fields, fields values, health check, menu, schemas, session, tags, user group map, user notes, user profiles, usergroups, users, or making API calls to https://joomla.augur-api.com.
version: 1.0.3
---

# Joomla

Service-specific knowledge for joomla microservice.

## API Documentation

- [OpenAPI Specification](https://joomla.augur-api.com/openapi.json)
- [Postman Collection](https://joomla.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### content

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /content/{id} | Get Content Detail | [content.md](content.md#get-contentid) |
| GET | /content/{id}/doc | Get Content Doc | [content.md](content.md#get-contentiddoc) |
| GET | /content | Get Content List | [content.md](content.md#get-content) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### menu

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /menu/{id}/doc | Get Menu Doc | [menu.md](menu.md#get-menuiddoc) |

### tags

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /tags | Get Tag List | [tags.md](tags.md#get-tags) |

### user_group_map

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /users/:id/groups/:groupId | get User Group | [user_group_map.md](user_group_map.md#get-users:idgroups:groupId) |
| GET | /users/:id/groups | List User Groups | [user_group_map.md](user_group_map.md#get-users:idgroups) |
| POST | /users/:id/groups | Create/update User Group Mapping | [user_group_map.md](user_group_map.md#post-users:idgroups) |

### usergroups

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /usergroups | Get User Groups | [usergroups.md](usergroups.md#get-usergroups) |

### users

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /users/{id} | Get User Detail | [users.md](users.md#get-usersid) |
| PUT | /users/{id} | Update user | [users.md](users.md#put-usersid) |
| DELETE | /users/{id} | BLOCK user | [users.md](users.md#delete-usersid) |
| GET | /users/{id}/doc | Get User Doc | [users.md](users.md#get-usersiddoc) |
| GET | /users/{id}/trinity | Get Trinity User Doc | [users.md](users.md#get-usersidtrinity) |
| GET | /users | Get User List | [users.md](users.md#get-users) |
| POST | /users | Create a user | [users.md](users.md#post-users) |
| POST | /users/verify-password | Verify the password for a user | [users.md](users.md#post-usersverify-password) |
