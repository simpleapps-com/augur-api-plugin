# Chat Gpt

Datatype for gregorovich microservice.

## GET /chat-gpt/ask

ChatGPT Ask

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| question | query | Yes | string | The question to ask |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
