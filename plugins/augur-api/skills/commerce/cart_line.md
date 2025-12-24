# Cart Line

Datatype for commerce microservice.

## GET /cart-line/{cartHdrUid}

GET Cart Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cart_hdr_uid | path | Yes | integer | cart_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /cart-line/{cartHdrUid}

DELETE Cart Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cart_hdr_uid | path | Yes | integer | cart_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /cart-line/{cartHdrUid}/add

ADD item to the cart

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cart_hdr_uid | path | Yes | integer | cart_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## DELETE /cart-line/{cartHdrUid}/lines/{lineNo}

DELETE a specific Cart Line

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cart_hdr_uid | path | Yes | integer | cart_hdr_uid |
| line_no | path | Yes | integer | line_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## POST /cart-line/{cartHdrUid}/update

UPDATE item to the cart

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| cart_hdr_uid | path | Yes | integer | cart_hdr_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
