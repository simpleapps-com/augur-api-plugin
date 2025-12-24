# Oe Pick Ticket

Datatype for orders microservice.

## GET /pick-tickets/{pickTicketNo}

Get Pick Ticket Details

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| pick_ticket_no | path | Yes | number | pick_ticket_no |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---

## GET /pick-tickets

List Pick Tickets

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| companyId | query | No | string | Company ID |
| deleteFlag | query | No | string | Delete Flag |
| limit | query | No | int | Limit number of results (Default: 10) |
| locationId | query | No | number | Location ID |
| offset | query | No | int | Starting offset results (Default: 0) |
| orderBy | query | No | string | Order By (Default: pick_ticket_no|ASC) |
| orderNo | query | No | string | Order Number |
| printedFlag | query | No | string | Printed Flag |
| q | query | No | string | Search Query |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
