---
name: Commerce API
description: Use when working with cart hdr, cart line, checkout, checkout legacy, checkout prophet21 hdr, checkout prophet21 line, health check, seed, or making API calls to https://commerce.augur-api.com.
version: 1.0.3
---

# Commerce

Service-specific knowledge for commerce microservice.

## API Documentation

- [OpenAPI Specification](https://commerce.augur-api.com/openapi.json)
- [Postman Collection](https://commerce.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### cart_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /cart-hdr/list | List Cart Hdr by user_id | [cart_hdr.md](cart_hdr.md#get-cart-hdrlist) |
| GET | /cart-hdr/lookup | Lookup Cart Hdr | [cart_hdr.md](cart_hdr.md#get-cart-hdrlookup) |
| GET | /cart-hdr/{cartHdrUid}/also-bought | List Also Bought data for Cart Hdr | [cart_hdr.md](cart_hdr.md#get-cart-hdrcartHdrUidalso-bought) |

### cart_line

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /cart-line/{cartHdrUid} | GET Cart Lines | [cart_line.md](cart_line.md#get-cart-linecartHdrUid) |
| DELETE | /cart-line/{cartHdrUid} | DELETE Cart Lines | [cart_line.md](cart_line.md#delete-cart-linecartHdrUid) |
| POST | /cart-line/{cartHdrUid}/add | ADD item to the cart | [cart_line.md](cart_line.md#post-cart-linecartHdrUidadd) |
| DELETE | /cart-line/{cartHdrUid}/lines/{lineNo} | DELETE a specific Cart Line | [cart_line.md](cart_line.md#delete-cart-linecartHdrUidlineslineNo) |
| POST | /cart-line/{cartHdrUid}/update | UPDATE item to the cart | [cart_line.md](cart_line.md#post-cart-linecartHdrUidupdate) |

### checkout

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /checkout | Create new Checkout | [checkout.md](checkout.md#post-checkout) |
| GET | /checkout/{checkoutUid} | Get Checkout Details | [checkout.md](checkout.md#get-checkoutcheckoutUid) |
| PUT | /checkout/{checkoutUid}/activate | Activate Checkout | [checkout.md](checkout.md#put-checkoutcheckoutUidactivate) |
| GET | /checkout/{checkoutUid}/doc | Get Checkout Doc | [checkout.md](checkout.md#get-checkoutcheckoutUiddoc) |
| PUT | /checkout/{checkoutUid}/validate | Validate Checkout | [checkout.md](checkout.md#put-checkoutcheckoutUidvalidate) |

### checkout_prophet21_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /checkout/{checkoutUid}/prophet21-hdr | Create new P21 Checkout | [checkout_prophet21_hdr.md](checkout_prophet21_hdr.md#post-checkoutcheckoutUidprophet21-hdr) |

### checkout_prophet21_line

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /checkout/{checkoutUid}/prophet21-hdr/{prophet21HdrUid}/prophet21-line | Add items to Prophet 21 checkout | [checkout_prophet21_line.md](checkout_prophet21_line.md#post-checkoutcheckoutUidprophet21-hdrprophet21HdrUidprophet21-line) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
