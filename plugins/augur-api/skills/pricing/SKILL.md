---
name: Pricing API
description: Use when working with health check, job price bin, job price customer shipto, job price hdr, job price line, legacy api price, price book, price book x library, price check, price engine, price engine calc, price family, price family x restricted class, price library, price library x cust x cmpy, price method x customer, price page, price page dealer commission, price page item, price page po cost calc, price page pricefam, price page prodgrp, price page secondary rebate, price page suppdisc, price page supplier, price page type x company, price page x book, price source x company, seed, sync tracking hdr, sync tracking line, tax engine, tax group hdr, tax group hdr zip, tax group line, tax jurisdiction, or making API calls to https://pricing.augur-api.com.
version: 1.0.4
---

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
