# Scheduled Import Metadata

Datatype for p21_sism microservice.

## POST /scheduled-import-master/{scheduled_import_master_uid}/metadata/sftp

Create SFTP metadata for a scheduled import master

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| scheduled_import_master_uid | path | Yes | string | scheduled_import_master.scheduled_import_master_uid |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
