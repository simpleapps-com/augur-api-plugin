# Shipvia

Datatype for logistics microservice.

## GET /shipvia/rates

Get ShipVia shipping rates from multiple carriers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| carriers | query | No | string | (Optional) Carrier filter: "standard" for UPS/FedEx/USPS, "UPS,FEDEX" for specific carriers, or omit for all carriers |
| dimensionUnit | query | No | string | (Optional) Dimension unit (IN or CM) |
| fromCity | query | No | string | (Optional) Origin city |
| fromCountry | query | No | string | (Optional) Origin country code (2-letter, default: US) |
| fromPostalCode | query | Yes | string | (Required) Origin postal/ZIP code |
| fromState | query | No | string | (Optional) Origin state/province (2-letter code) |
| locationId | query | Yes | integer | (Required) ShipVia location ID |
| packageHeight | query | No | number | (Optional) Package height |
| packageLength | query | No | number | (Optional) Package length |
| packageWidth | query | No | number | (Optional) Package width |
| residential | query | No | boolean | (Optional) Residential delivery flag (default: true) |
| serviceType | query | No | string | (Optional) Service type filter: ground, express, or overnight |
| toCity | query | No | string | (Optional) Destination city |
| toCountry | query | No | string | (Optional) Destination country code (2-letter, default: US) |
| toPostalCode | query | Yes | string | (Required) Destination postal/ZIP code |
| toState | query | No | string | (Optional) Destination state/province (2-letter code) |
| totalWeight | query | Yes | number | (Required) Total package weight |
| weightUnit | query | Yes | string | (Required) Weight unit (LBS or KG) |
| x-site-id | header | Yes | string | Site ID provided by SimpleApps |

---

## GET /shipvia/rates/ltl

Get ShipVia LTL (Less-Than-Truckload) freight rates from multiple carriers

### Parameters

| Name | Location | Required | Type | Description |
|------|----------|----------|------|-------------|
| Authorization | header | Yes | string | Bearer token (JWT) |
| carriers | query | No | string | (Optional) Carrier filter: "standard" for major LTL carriers, "FEDEX_FREIGHT,UPS_FREIGHT" for specific carriers, or omit for all LTL carriers |
| commodityClass | query | Yes | string | (Required) NMFC freight class: 50, 55, 60, 65, 70, 77.5, 85, 92.5, 100, 110, 125, 150, 175, 200, 250, 300, 400, 500 |
| commodityDescription | query | Yes | string | (Required) Description of commodity being shipped |
| deliveryInstructions | query | No | string | (Optional) Special delivery instructions (liftgate, inside delivery, etc.) |
| dimensionUnit | query | No | string | (Optional) Dimension unit (IN or CM, default: IN) |
| fromCity | query | No | string | (Optional) Origin city |
| fromCountry | query | No | string | (Optional) Origin country code (2-letter, default: US) |
| fromPostalCode | query | Yes | string | (Required) Origin postal/ZIP code |
| fromState | query | No | string | (Optional) Origin state/province (2-letter code) |
| isHazMat | query | No | boolean | (Optional) Hazardous materials flag (default: false) |
| locationId | query | Yes | integer | (Required) ShipVia location ID |
| packageHeight | query | No | number | (Optional) Freight height |
| packageLength | query | No | number | (Optional) Freight length |
| packageWidth | query | No | number | (Optional) Freight width |
| packagingType | query | Yes | string | (Required) Packaging type: PALLET, CRATE, CARTON, DRUM, BUNDLE, BAG, BOX, SKID |
| pickupInstructions | query | No | string | (Optional) Special pickup instructions (liftgate required, loading dock, etc.) |
| quantity | query | No | integer | (Optional) Number of handling units (default: 1) |
| toCity | query | No | string | (Optional) Destination city |
| toCountry | query | No | string | (Optional) Destination country code (2-letter, default: US) |
| toPostalCode | query | Yes | string | (Required) Destination postal/ZIP code |
| toState | query | No | string | (Optional) Destination state/province (2-letter code) |
| totalWeight | query | Yes | number | (Required) Total freight weight (typically 150+ lbs) |
| weightUnit | query | Yes | string | (Required) Weight unit (LBS or KG) |
| x-site-id | header | Yes | string | Site ID provided by SimpleApps |

---
