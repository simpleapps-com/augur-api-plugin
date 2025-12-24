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
