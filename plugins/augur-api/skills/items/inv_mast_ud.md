# Inv Mast Ud

Datatype for items microservice.

## GET /inv-mast-ud

List inv_mast_ud records with filtering and pagination

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| createdSince | query | No | string | Filter by date_created since date (YYYY-MM-DD HH:MM:SS) |
| invMastUdUid | query | No | int | Filter by inv_mast_ud_uid |
| invMastUid | query | No | int | Filter by inv_mast_uid |
| limit | query | No | int | Maximum number of records to return |
| modifiedSince | query | No | string | Filter by date_last_modified since date (YYYY-MM-DD HH:MM:SS) |
| offset | query | No | int | Number of records to skip |
| orderBy | query | No | string | Order by field and direction (e.g., inv_mast_ud_uid|DESC) |
| statusCd | query | No | int | Filter by status_cd |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
