---
name: Legacy API
description: Use when working with address, also bought, alternate code, attrib items, attrib names, attrib names x attrib values, attrib names x item category, attrib values, branch, code p21, company, contacts, contacts x ship to, coupons, creditcard processor, ctl inv mast hazmat detail, customer, customer pastpurchase, health check, inv accessory, inv loc, inv loc stock status, inv mast, inv mast 15, inv mast attributes, inv mast links, inv mast meta, inv mast msds, inv mast primarysupplier, inv mast tags, inv mast ud, inv mast web desc, inv mast x restricted class, inv period usage, inv sub, inv xref, inventory supplier, inventory supplier x loc, item category, item category hierarchy, item category hierarchy delete audit, item category image, item category link, item category set, item category text, item category x inv mast, item conversion, item options hdr, item options line, item package type, item personalization hdr, item personalization line, item uom, job price bin, job price customer shipto, job price hdr, job price line, job price value, location, messages, modified dates, modified pricing, oe hdr, oe hdr notepad, oe line, oe line labor, oe line service labor, oe pick ticket, orders, package type, packing basis, payment types, price family, profit sharing, seed, service labor, service labor rate, service technician, service technician x labor, ship to, ship to salesrep, ship to ud, state, system setting, terms, unit of measure, users, web display type, web orders meta, or making API calls to https://legacy.augur-api.com.
version: 1.0.3
---

# Legacy

Service-specific knowledge for legacy microservice.

## API Documentation

- [OpenAPI Specification](https://legacy.augur-api.com/openapi.json)
- [Postman Collection](https://legacy.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### also_bought

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/also-bought | List item Also Bought | [also_bought.md](also_bought.md#get-inv-mastinvMastUidalso-bought) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### inv_mast_tags

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/:invMastUid/tags/:invMastTagsUid | Get Inv Mast Tag Details | [inv_mast_tags.md](inv_mast_tags.md#get-inv-mast:invMastUidtags:invMastTagsUid) |
| PUT | /inv-mast/:invMastUid/tags/:invMastTagsUid | Update Inv Mast Tag | [inv_mast_tags.md](inv_mast_tags.md#put-inv-mast:invMastUidtags:invMastTagsUid) |
| DELETE | /inv-mast/:invMastUid/tags/:invMastTagsUid | Delete Inv Mast Tag | [inv_mast_tags.md](inv_mast_tags.md#delete-inv-mast:invMastUidtags:invMastTagsUid) |
| GET | /inv-mast/:invMastUid/tags | List Inv Mast Tags | [inv_mast_tags.md](inv_mast_tags.md#get-inv-mast:invMastUidtags) |
| POST | /inv-mast/:invMastUid/tags | Create Inv Mast Tag | [inv_mast_tags.md](inv_mast_tags.md#post-inv-mast:invMastUidtags) |

### inv_mast_web_desc

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/web-desc/{invMastWebDescUid} | Get Item Web Description | [inv_mast_web_desc.md](inv_mast_web_desc.md#get-inv-mastinvMastUidweb-descinvMastWebDescUid) |
| PUT | /inv-mast/{invMastUid}/web-desc/{invMastWebDescUid} | Update Item Web Description | [inv_mast_web_desc.md](inv_mast_web_desc.md#put-inv-mastinvMastUidweb-descinvMastWebDescUid) |
| DELETE | /inv-mast/{invMastUid}/web-desc/{invMastWebDescUid} | Delete Item Web Description | [inv_mast_web_desc.md](inv_mast_web_desc.md#delete-inv-mastinvMastUidweb-descinvMastWebDescUid) |
| GET | /inv-mast/{invMastUid}/web-desc | List item Web Descriptions | [inv_mast_web_desc.md](inv_mast_web_desc.md#get-inv-mastinvMastUidweb-desc) |
| POST | /inv-mast/{invMastUid}/web-desc | Create Web Description for Item | [inv_mast_web_desc.md](inv_mast_web_desc.md#post-inv-mastinvMastUidweb-desc) |

### item_category

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-category/{itemCategoryUid} | Get Item Category Details | [item_category.md](item_category.md#get-item-categoryitemCategoryUid) |

### orders

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /orders/{id}/reset | Reset orders for processing by id | [orders.md](orders.md#get-ordersidreset) |

### state

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /legacy/state/{stateUid} | Get State Details | [state.md](state.md#get-legacystatestateUid) |
| PUT | /legacy/state/{stateUid} | Update State | [state.md](state.md#put-legacystatestateUid) |
| DELETE | /legacy/state/{stateUid} | DELETE State | [state.md](state.md#delete-legacystatestateUid) |
| GET | /legacy/state | List States | [state.md](state.md#get-legacystate) |
| POST | /legacy/state | Create State | [state.md](state.md#post-legacystate) |
