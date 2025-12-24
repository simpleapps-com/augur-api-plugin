# Oe Pick Ticket Detail

Datatype for orders microservice.

## GET /pick-tickets/{pickTicketNo}/lines/{lineNumber}

Get Pick Ticket Line Detail

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| line_number | path | Yes | number | line_number |
| pick_ticket_no | path | Yes | number | pick_ticket_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /pick-tickets/{pickTicketNo}/lines

List Pick Ticket Lines

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| limit | query | No | int | Limit number of results (Default: 10) |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: line_number|ASC) |
| pick_ticket_no | path | Yes | number | pick_ticket_no |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
