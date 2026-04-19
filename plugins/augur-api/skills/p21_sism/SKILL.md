---
name: P21 Sism API
description: Use when working with cc tables, health check, imp address, imp ar payment details, imp ar receipts, imp ar receipts detail, imp contacts, imp creditcard payment details, imp customer, imp customer notepad, imp document line bin, imp document line lot, imp document line lot bin xref, imp document line serial, imp finished good lot, imp inv adj hdr, imp inv adj line, imp inv ret ship hdr, imp inv ret ship line, imp inventory receipt attribute value, imp inventory receipts hdr, imp lot x lot attribute value, imp note area, imp note area oe line, imp oe hdr, imp oe hdr notepad, imp oe hdr salesrep, imp oe hdr web, imp oe line, imp oe line notepad, imp oe line schedule, imp oe line service, imp oe line service labor, imp oe line service labor time, imp oe line service part, imp oe pick ticket, imp oe pick ticket detail, imp oe po xref, imp oe schedule, imp oe schedule detail, imp po hdr, imp po hdr notepad, imp po line, imp po line notepad, imp prod order hdr, imp prod order line, imp prod order line comp labor, imp prod order line component, imp rebate payments detail, imp rma receipt hdr import, imp rma receipt line import, imp ship to, imp tag document line, imp tag hdr, imp transfer hdr, imp transfer line, imp transfer ship hdr, imp transfer ship line, impexp source, import, import suspense settings, scheduled import def, scheduled import details, scheduled import master, scheduled import metadata, seed, transaction set, or making API calls to https://p21-sism.augur-api.com.
version: 1.0.5
---

# P21 Sism

Service-specific knowledge for p21_sism microservice.

## API Documentation

- [OpenAPI Specification](https://p21-sism.augur-api.com/openapi.json)
- [Postman Collection](https://p21-sism.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |

### imp_oe_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /import/{importUid}/imp-oe-hdr | Get the details from imp_oe_hdr table | [imp_oe_hdr.md](imp_oe_hdr.md#get-importimportUidimp-oe-hdr) |
| PUT | /import/{importUid}/imp-oe-hdr | Update imp_oe_hdr table | [imp_oe_hdr.md](imp_oe_hdr.md#put-importimportUidimp-oe-hdr) |

### imp_oe_hdr_salesrep

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /import/{importUid}/imp-oe-hdr-salesrep | Get the details from imp_oe_hdr_salesrep table | [imp_oe_hdr_salesrep.md](imp_oe_hdr_salesrep.md#get-importimportUidimp-oe-hdr-salesrep) |
| PUT | /import/{importUid}/imp-oe-hdr-salesrep | Update imp_oe_hdr_salesrep table | [imp_oe_hdr_salesrep.md](imp_oe_hdr_salesrep.md#put-importimportUidimp-oe-hdr-salesrep) |

### imp_oe_hdr_web

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /import/{importUid}/imp-oe-hdr-web | Get the details from imp_oe_hdr_web table | [imp_oe_hdr_web.md](imp_oe_hdr_web.md#get-importimportUidimp-oe-hdr-web) |

### import

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /import/daily-summary | Get daily import counts by state | [import.md](import.md#get-importdaily-summary) |
| GET | /import/{importUid} | Get the details of an import | [import.md](import.md#get-importimportUid) |
| PUT | /import/{importUid} | Update an import | [import.md](import.md#put-importimportUid) |
| DELETE | /import/{importUid} | clean pending_import for an import | [import.md](import.md#delete-importimportUid) |
| GET | /import | Get a list of imports | [import.md](import.md#get-import) |
| GET | /import/recent | Get a list of the most recent imports | [import.md](import.md#get-importrecent) |
| GET | /import/stuck | Get a list of stuck imports | [import.md](import.md#get-importstuck) |

### scheduled_import_metadata

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /scheduled-import-master/{scheduledImportMasterUid}/metadata/sftp | Create SFTP metadata for a scheduled import master | [scheduled_import_metadata.md](scheduled_import_metadata.md#post-scheduled-import-masterscheduledImportMasterUidmetadatasftp) |
