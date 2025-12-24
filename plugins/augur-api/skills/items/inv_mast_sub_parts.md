# Inv Mast Sub Parts

Datatype for items microservice.

## GET /inv-mast-sub-parts/{invMastUid}

List sub parts for an item

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| invMastLinksUid | query | No | integer | inv_mast_link.inv_mast_links_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
