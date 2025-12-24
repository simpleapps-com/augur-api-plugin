# Usergroups

Datatype for joomla microservice.

## GET /usergroups

Get User Groups

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| orderBy | query | No | string | Select order of the groups Default: title|ASC |
| parentIdList | query | No | string | CSV List of parent ids (default:blank) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
