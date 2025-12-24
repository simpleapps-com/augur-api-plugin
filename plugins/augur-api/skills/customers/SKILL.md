---
name: Customers API
description: Use when working with contact role, contacts, contacts ud, contacts x ship to, customer, customer language, customer ud, customer x restricted class, health check, invoices, oe contacts customer, orders, purchased items, quotes, rewards program, seed, ship to, ship to ud, sync tracking hdr, sync tracking line, or making API calls to https://customers.augur-api.com.
version: 1.0.2
---

# Customers

Service-specific knowledge for customers microservice.

## API Documentation

- [OpenAPI Specification](https://customers.augur-api.com/openapi.json)
- [Postman Collection](https://customers.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### contacts

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /contacts/{id}/customers | List Salesrep Customers | [contacts.md](contacts.md#get-contactsidcustomers) |
| GET | /contacts/{id}/doc | get the contact document | [contacts.md](contacts.md#get-contactsiddoc) |
| GET | /contacts/{id}/web-allowance | Get the web allowance for a contact_id (USCCO) | [contacts.md](contacts.md#get-contactsidweb-allowance) |
| GET | /contacts/refresh | Trigger a data refresh | [contacts.md](contacts.md#get-contactsrefresh) |

### contacts_ud

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /contacts-ud/{id} | List user defined fields for a contact | [contacts_ud.md](contacts_ud.md#get-contacts-udid) |

### customer

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /customer/{customerId}/address | Lookup Customer Addresses | [customer.md](customer.md#get-customercustomerIdaddress) |
| GET | /customer/{customerId}/contacts | Lookup Customer Contacts | [customer.md](customer.md#get-customercustomerIdcontacts) |
| POST | /customer/{customerId}/contacts | Create new contact for customer_id | [customer.md](customer.md#post-customercustomerIdcontacts) |
| GET | /customer/{customerId}/doc | get the customer document | [customer.md](customer.md#get-customercustomerIddoc) |
| GET | /customer/{customerId}/ship-to | Lookup Customer ShipTo | [customer.md](customer.md#get-customercustomerIdship-to) |
| POST | /customer/{customerId}/ship-to | Create new ship_to for customer_id | [customer.md](customer.md#post-customercustomerIdship-to) |
| GET | /customer | list the customer documents | [customer.md](customer.md#get-customer) |
| GET | /customer/lookup | Lookup Customer summary | [customer.md](customer.md#get-customerlookup) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### invoices

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /customer/{customerId}/invoices/{invoiceNo} | Get Customer Invoice | [invoices.md](invoices.md#get-customercustomerIdinvoicesinvoiceNo) |
| GET | /customer/{customerId}/invoices | List Customer Invoices | [invoices.md](invoices.md#get-customercustomerIdinvoices) |

### oe_contacts_customer

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /oe-contacts-customer/refresh | Trigger a data refresh | [oe_contacts_customer.md](oe_contacts_customer.md#get-oe-contacts-customerrefresh) |

### orders

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /customer/{customerId}/orders/{orderNo} | Get Customer Order | [orders.md](orders.md#get-customercustomerIdordersorderNo) |
| GET | /customer/{customerId}/orders | List Customer Orders | [orders.md](orders.md#get-customercustomerIdorders) |

### purchased_items

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /customer/{customerId}/purchased-items | List Customer Purchased Items | [purchased_items.md](purchased_items.md#get-customercustomerIdpurchased-items) |

### quotes

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /customer/{customerId}/quotes/{quoteNo} | Get Customer Quote | [quotes.md](quotes.md#get-customercustomerIdquotesquoteNo) |
| GET | /customer/{customerId}/quotes | List Customer Quotes | [quotes.md](quotes.md#get-customercustomerIdquotes) |

### ship_to

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /customer/{customerId}/ship-to | List Customer Ship-To Addresses | [ship_to.md](ship_to.md#get-customercustomerIdship-to) |
| GET | /ship-to/refresh | Trigger a data refresh | [ship_to.md](ship_to.md#get-ship-torefresh) |
