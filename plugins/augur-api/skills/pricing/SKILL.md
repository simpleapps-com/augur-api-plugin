# Pricing

Service-specific knowledge for pricing microservice.

## API Documentation

- [OpenAPI Specification](https://pricing.augur-api.com/openapi.json)
- [Postman Collection](https://pricing.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### job_price_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /job-price-hdr/{jobPriceHdrUid} | Get Job Price Header Details | [job_price_hdr.md](job_price_hdr.md#get-job-price-hdrjobPriceHdrUid) |
| GET | /job-price-hdr | List Job Price Headers | [job_price_hdr.md](job_price_hdr.md#get-job-price-hdr) |

### job_price_line

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /job-price-hdr/{jobPriceHdrUid}/lines/{jobPriceLineUid} | Get Job Price Line Details | [job_price_line.md](job_price_line.md#get-job-price-hdrjobPriceHdrUidlinesjobPriceLineUid) |
| GET | /job-price-hdr/{jobPriceHdrUid}/lines | List Job Price Lines | [job_price_line.md](job_price_line.md#get-job-price-hdrjobPriceHdrUidlines) |

### price_engine

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /price-engine | Get Item Price | [price_engine.md](price_engine.md#get-price-engine) |

### tax_engine

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /tax-engine | Run Tax Engine | [tax_engine.md](tax_engine.md#post-tax-engine) |
