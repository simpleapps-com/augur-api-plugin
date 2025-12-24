# Authentication

All API endpoints except `/health-check` and `/ping` require a bearer token.

## Header Format

```
Authorization: Bearer {token}
x-site-id: {siteId}
```

## Token Type

JWT (JSON Web Token)

## Obtaining a Token

Contact the SimpleApps team for API credentials. Tokens are issued for security and are specific to your organization.
