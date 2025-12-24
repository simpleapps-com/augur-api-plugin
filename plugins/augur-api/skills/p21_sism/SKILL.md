---
name: P21 Sism API
description: Use when working with cc tables, health check, imp address, imp ar payment details, imp ar receipts, imp ar receipts detail, imp contacts, imp creditcard payment details, imp customer, imp customer notepad, imp document line bin, imp document line lot, imp document line lot bin xref, imp document line serial, imp finished good lot, imp inv adj hdr, imp inv adj line, imp inv ret ship hdr, imp inv ret ship line, imp inventory receipt attribute value, imp inventory receipts hdr, imp lot x lot attribute value, imp note area, imp note area oe line, imp oe hdr, imp oe hdr notepad, imp oe hdr salesrep, imp oe hdr web, imp oe line, imp oe line notepad, imp oe line schedule, imp oe line service, imp oe line service labor, imp oe line service labor time, imp oe line service part, imp oe pick ticket, imp oe pick ticket detail, imp oe po xref, imp oe schedule, imp oe schedule detail, imp po hdr, imp po hdr notepad, imp po line, imp po line notepad, imp prod order hdr, imp prod order line, imp prod order line comp labor, imp prod order line component, imp rebate payments detail, imp rma receipt hdr import, imp rma receipt line import, imp ship to, imp tag document line, imp tag hdr, imp transfer hdr, imp transfer line, imp transfer ship hdr, imp transfer ship line, impexp source, import, import suspense settings, scheduled import def, scheduled import details, scheduled import master, scheduled import metadata, seed, transaction set, or making API calls to https://p21-sism.augur-api.com.
version: 1.0.1
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
| GET | /import/{import_uid}/imp-oe-hdr | Get the details from imp_oe_hdr table | [imp_oe_hdr.md](imp_oe_hdr.md#get-importimport_uidimp-oe-hdr) |
| PUT | /import/{import_uid}/imp-oe-hdr | Update imp_oe_hdr table | [imp_oe_hdr.md](imp_oe_hdr.md#put-importimport_uidimp-oe-hdr) |

### imp_oe_hdr_salesrep

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /import/{import_uid}/imp-oe-hdr-salesrep | Get the details from imp_oe_hdr_salesrep table | [imp_oe_hdr_salesrep.md](imp_oe_hdr_salesrep.md#get-importimport_uidimp-oe-hdr-salesrep) |
| PUT | /import/{import_uid}/imp-oe-hdr-salesrep | Update imp_oe_hdr_salesrep table | [imp_oe_hdr_salesrep.md](imp_oe_hdr_salesrep.md#put-importimport_uidimp-oe-hdr-salesrep) |

### imp_oe_hdr_web

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /import/{import_uid}/imp-oe-hdr-web | Get the details from imp_oe_hdr_web table | [imp_oe_hdr_web.md](imp_oe_hdr_web.md#get-importimport_uidimp-oe-hdr-web) |

### imp_oe_line

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /imp_oe_line/{importUid}/{lineNo} | Get ImpOeLine Details | [imp_oe_line.md](imp_oe_line.md#get-imp_oe_lineimportUidlineNo) |
| PUT | /imp_oe_line/{importUid}/{lineNo} | Update ImpOeLine | [imp_oe_line.md](imp_oe_line.md#put-imp_oe_lineimportUidlineNo) |
| GET | /imp_oe_line | List ImpOeLines | [imp_oe_line.md](imp_oe_line.md#get-imp_oe_line) |

### import

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /import/{import_uid} | Get the details of an import | [import.md](import.md#get-importimport_uid) |
| PUT | /import/{import_uid} | Update an import | [import.md](import.md#put-importimport_uid) |
| DELETE | /import/{import_uid} | clean pending_import for an import | [import.md](import.md#delete-importimport_uid) |
| GET | /import | Get a list of imports | [import.md](import.md#get-import) |
| GET | /import/recent | Get a list of the most recent imports | [import.md](import.md#get-importrecent) |
| GET | /import/stuck | Get a list of stuck imports | [import.md](import.md#get-importstuck) |

### scheduled_import_metadata

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /scheduled-import-master/{scheduled_import_master_uid}/metadata/sftp | Create SFTP metadata for a scheduled import master | [scheduled_import_metadata.md](scheduled_import_metadata.md#post-scheduled-import-masterscheduled_import_master_uidmetadatasftp) |
