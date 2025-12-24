# Augur API Plugin for Claude Code

Claude Code plugin providing API documentation skills for Augur microservices.

## Installation

```bash
# Add the marketplace
claude /plugin marketplace add simpleapps-com/augur-api-plugin

# Install the plugin
claude /plugin install augur-api@augur-api
```

## Available Skills

This plugin provides 27 service-specific skills with API endpoint documentation:

| Service | Description |
|---------|-------------|
| agr_info | Augur information and system metadata |
| agr_site | Site configuration and settings |
| agr_work | Work queue and job management |
| avalara | Tax calculation (Avalara integration) |
| basecamp2 | Basecamp API integration |
| brand_folder | Brand asset management |
| commerce | Shopping cart and checkout |
| customers | Customer management and contacts |
| gregorovich | AI/LLM integration (ChatGPT, Ollama) |
| items | Product catalog and inventory |
| joomla | Joomla CMS integration |
| legacy | Legacy system compatibility |
| logistics | Shipping and fulfillment |
| nexus | Warehouse transfers and receiving |
| open_search | Search and suggestions |
| orders | Order management |
| p21_apis | Prophet 21 API endpoints |
| p21_core | Prophet 21 core entities |
| p21_pim | Prophet 21 product information |
| p21_sism | Prophet 21 sales import |
| payments | Payment processing |
| pricing | Price and tax calculations |
| shipping | Shipping rates |
| slack | Slack notifications |
| smarty_streets | Address validation |
| ups | UPS shipping rates |
| vmi | Vendor managed inventory |

## Authentication

All API endpoints (except `/health-check` and `/ping`) require bearer token authentication:

```
Authorization: Bearer <jwt-token>
```

See the `authentication.md` skill for details on obtaining tokens.

## API Documentation Formats

Each service provides:
- OpenAPI specification: `https://{service}.augur-api.com/openapi.json`
- Postman collection: `https://{service}.augur-api.com/postman.json`

## Usage

Once installed, Claude Code automatically loads relevant skills when you:
- Ask about specific API endpoints
- Work with service-specific datatypes
- Need to make API calls to Augur services

## Version

1.0.4

## License

Proprietary - SimpleApps
