# Orders

Service-specific knowledge for orders microservice.

## API Documentation

- [OpenAPI Specification](https://orders.augur-api.com/openapi.json)
- [Postman Collection](https://orders.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### invoice_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /invoice-hdr/{invoiceNo}/reprint | Reprint the invoice | [invoice_hdr.md](invoice_hdr.md#get-invoice-hdrinvoiceNoreprint) |

### oe_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /oe-hdr/lookup | Lookup OeHdr summary | [oe_hdr.md](oe_hdr.md#get-oe-hdrlookup) |
| GET | /oe-hdr/{orderNo}/doc | get the order document | [oe_hdr.md](oe_hdr.md#get-oe-hdrorderNodoc) |

### oe_hdr_salesrep

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /oe-hdr-salesrep/{salesrep-id}/oe-hdr | get oe_hdr data for salesrep | [oe_hdr_salesrep.md](oe_hdr_salesrep.md#get-oe-hdr-salesrepsalesrep-idoe-hdr) |
| GET | /oe-hdr-salesrep/{salesrep_id}/oe-hdr/{orderNo}/doc | get oe_hdr details for salesrep | [oe_hdr_salesrep.md](oe_hdr_salesrep.md#get-oe-hdr-salesrepsalesrep_idoe-hdrorderNodoc) |

### oe_pick_ticket

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /pick-tickets/{pickTicketNo} | Get Pick Ticket Details | [oe_pick_ticket.md](oe_pick_ticket.md#get-pick-ticketspickTicketNo) |
| GET | /pick-tickets | List Pick Tickets | [oe_pick_ticket.md](oe_pick_ticket.md#get-pick-tickets) |

### oe_pick_ticket_detail

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /pick-tickets/{pickTicketNo}/lines/{lineNumber} | Get Pick Ticket Line Detail | [oe_pick_ticket_detail.md](oe_pick_ticket_detail.md#get-pick-ticketspickTicketNolineslineNumber) |
| GET | /pick-tickets/{pickTicketNo}/lines | List Pick Ticket Lines | [oe_pick_ticket_detail.md](oe_pick_ticket_detail.md#get-pick-ticketspickTicketNolines) |

### po_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /po-hdr/{poNo} | get the purchase order details | [po_hdr.md](po_hdr.md#get-po-hdrpoNo) |
| GET | /po-hdr/{poNo}/doc | get the purchase order document | [po_hdr.md](po_hdr.md#get-po-hdrpoNodoc) |
| GET | /po-hdr | Lookup PoHdr | [po_hdr.md](po_hdr.md#get-po-hdr) |
| POST | /po-hdr/scan | Scan for similar purchase orders based on criteria | [po_hdr.md](po_hdr.md#post-po-hdrscan) |
