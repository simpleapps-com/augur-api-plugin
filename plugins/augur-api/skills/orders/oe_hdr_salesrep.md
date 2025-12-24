# Oe Hdr Salesrep

Datatype for orders microservice.

## GET /oe-hdr-salesrep/{salesrep-id}/oe-hdr

get oe_hdr data for salesrep

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| sales_rep_id | path | Yes | integer | oe_hdr_salesrep.salesrep_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /oe-hdr-salesrep/{salesrep_id}/oe-hdr/{orderNo}/doc

get oe_hdr details for salesrep

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| order_no | path | Yes | integer | oe_hdr.order_no |
| sales_rep_id | path | Yes | integer | oe_hdr_salesrep.salesrep_id |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
