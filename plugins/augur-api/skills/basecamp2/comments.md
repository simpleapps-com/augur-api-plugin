# Comments

Datatype for basecamp2 microservice.

## GET /comments/{id}

Get Comment by ID

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | Comment ID |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
