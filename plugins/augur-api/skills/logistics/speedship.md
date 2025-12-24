# Speedship

Datatype for logistics microservice.

## GET /speedship/freight

Get Speedship Freight

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| deliveryInstructions | query | No | string | (Optional) Special instructions for delivery(LTL only) |
| dimensionUnit | query | Yes | string | (Required) Dimension unit (IN) |
| fromAddressLine | query | Yes | string | (Required) From address line |
| fromCity | query | Yes | string | (Required) From city |
| fromCompanyName | query | Yes | string | (Required) From company name |
| fromCountryCode | query | Yes | string | (Required) From country code |
| fromFirstName | query | Yes | string | (Required) From first name |
| fromLastName | query | Yes | string | (Required) From last name |
| fromPhone | query | Yes | string | (Required) From phone |
| fromPostalCode | query | Yes | string | (Required) From postal code |
| fromState | query | Yes | string | (Required) From state |
| handlingCharge | query | No | number | (Optional) Handling charge amount |
| handlingChargeUnit | query | No | string | (Optional) Handling charge unit (PERCENT|AMOUNT) |
| international | query | No | boolean | (Optional) International flag |
| packageHeight | query | No | number | (Optional) Package height (IN) |
| packageLength | query | Yes | number | (Required) Package length (IN) |
| packageWidth | query | Yes | number | (Required) Package width (IN) |
| pickupInstructions | query | No | string | (Optional) Special instructions for pickup(LTL only) |
| productType | query | Yes | string | (Required) Product type (Default: LTL) | SMALLPACK |
| quantity | query | Yes | number | (Required) Packaging handling unit (Default: 1) |
| responseFormat | query | Yes | string | (Required) Response format (summary | detailed | cheapest | vendor) |
| toAddressLine | query | Yes | string | (Required) To address line |
| toCity | query | Yes | string | (Required) To city |
| toCompanyName | query | Yes | string | (Required) To company name |
| toCountryCode | query | Yes | string | (Required) To country code |
| toFirstName | query | Yes | string | (Required) To first name |
| toLastName | query | Yes | string | (Required) To last name |
| toPhone | query | Yes | string | (Required) To phone |
| toPostalCode | query | Yes | string | (Required) To postal code |
| toRegion | query | Yes | string | (Required) To region |
| totalWeight | query | Yes | number | (Required) Total weight of the shipment (LB) |
| weightUnit | query | Yes | string | (Required) Weight unit (LB) |
| x-site-id | header | Yes | string | siteId provided by SimpleApps |

---
