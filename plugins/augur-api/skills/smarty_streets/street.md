# Street

Datatype for smarty_streets microservice.

## GET /us/lookup

Lookup US Address

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| address1 | query | Yes | string | Address1 |
| address2 | query | Yes | string | Address2 |
| city | query | Yes | string | City |
| postalCode | query | Yes | string | Postal Code |
| state | query | Yes | string | State |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
