# Alternate Code

Datatype for items microservice.

## GET /inv-mast/{invMastUid}/alternate-code

List alternate codes

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv-mast-uid | path | Yes | integer | inv_mast.inv_mast_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
