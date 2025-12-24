# Invoice Hdr

Datatype for orders microservice.

## GET /invoice-hdr/{invoiceNo}/reprint

Reprint the invoice

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| invoice_no | path | Yes | integer | invoice_hdr.invoice_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
