# P21 Core

Service-specific knowledge for p21_core microservice.

## API Documentation

- [OpenAPI Specification](https://p21-core.augur-api.com/openapi.json)
- [Postman Collection](https://p21-core.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### address

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /address/{id} | Get Address Details | [address.md](address.md#get-addressid) |
| GET | /address/{id}/corp-address | Get Corporate Address List | [address.md](address.md#get-addressidcorp-address) |
| GET | /address/{id}/default | Set Address as default Shipping Method | [address.md](address.md#get-addressiddefault) |
| GET | /address/{id}/enable | Enable/disable Address as Shipping Method | [address.md](address.md#get-addressidenable) |
| GET | /address/refresh | Trigger a data refresh | [address.md](address.md#get-addressrefresh) |
| GET | /address | List Addresses | [address.md](address.md#get-address) |

### cash_drawer

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /cash_drawer/{cashDrawerUid} | Get Cash Drawer Details | [cash_drawer.md](cash_drawer.md#get-cash_drawercashDrawerUid) |
| GET | /cash_drawer | List Cash Drawers | [cash_drawer.md](cash_drawer.md#get-cash_drawer) |

### code_p21

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /code-p21 | List P21 Codes | [code_p21.md](code_p21.md#get-code-p21) |

### company

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /company/{companyUid} | Get Company Details | [company.md](company.md#get-companycompanyUid) |
| GET | /company | List Companies | [company.md](company.md#get-company) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### location

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /location/{locationId} | Get Location Details | [location.md](location.md#get-locationlocationId) |
| GET | /location | List Locations | [location.md](location.md#get-location) |

### payment_types

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /payment-types | List Payment Types | [payment_types.md](payment_types.md#get-payment-types) |
