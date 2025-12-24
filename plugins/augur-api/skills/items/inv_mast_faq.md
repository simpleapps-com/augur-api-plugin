# Inv Mast Faq

Datatype for items microservice.

## GET /inv-mast/{invMastUid}/faq/{invMastFaqUid}

Get Item FAQ Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_faq_uid | path | Yes | integer | inv_mast_faq_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## PUT /inv-mast/{invMastUid}/faq/{invMastFaqUid}

Update Item FAQ

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_faq_uid | path | Yes | integer | inv_mast_faq_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /inv-mast/{invMastUid}/faq/{invMastFaqUid}

DELETE Item FAQ

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_faq_uid | path | Yes | integer | inv_mast_faq_uid |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /inv-mast/{invMastUid}/faq

List Item FAQs

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: inv_mast_faq_uid|ASC) |
| q | query | No | string | Search Query |
| statusCd | query | No | int | Status Code (status_cd) [(704)|705|700|-1] |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /inv-mast/{invMastUid}/faq

Create Item FAQ

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| inv_mast_uid | path | Yes | integer | inv_mast.inv_mast_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
