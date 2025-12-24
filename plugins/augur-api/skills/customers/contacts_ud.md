# Contacts Ud

Datatype for customers microservice.

## GET /contacts-ud/{id}

List user defined fields for a contact

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| id | path | Yes | integer | contacts.id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
