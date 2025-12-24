---
name: Vmi API
description: Use when working with distributors, health check, inv profile hdr, inv profile line, inv warehouse, products, restock hdr, restock line, sections, seed, usage hdr, usage line, usage line warranty, warehouse, warehouse x users, or making API calls to https://vmi.augur-api.com.
version: 1.0.5
---

# Vmi

Service-specific knowledge for vmi microservice.

## API Documentation

- [OpenAPI Specification](https://vmi.augur-api.com/openapi.json)
- [Postman Collection](https://vmi.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### distributors

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /distributors/{distributorsUid} | Get distributor Details | [distributors.md](distributors.md#get-distributorsdistributorsUid) |
| PUT | /distributors/{distributorsUid} | Update distributor | [distributors.md](distributors.md#put-distributorsdistributorsUid) |
| DELETE | /distributors/{distributorsUid} | DELETE distributor | [distributors.md](distributors.md#delete-distributorsdistributorsUid) |
| PUT | /distributors/{distributorsUid}/enable | Enable/Disable/Delete distributor | [distributors.md](distributors.md#put-distributorsdistributorsUidenable) |
| GET | /distributors | List distributors | [distributors.md](distributors.md#get-distributors) |
| POST | /distributors | Create distributor | [distributors.md](distributors.md#post-distributors) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### inv_profile_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-profile-hdr/{invProfileHdrUid} | Get Inventory Profile Header Details | [inv_profile_hdr.md](inv_profile_hdr.md#get-inv-profile-hdrinvProfileHdrUid) |
| PUT | /inv-profile-hdr/{invProfileHdrUid} | Update Inventory Profile Header | [inv_profile_hdr.md](inv_profile_hdr.md#put-inv-profile-hdrinvProfileHdrUid) |
| DELETE | /inv-profile-hdr/{invProfileHdrUid} | DELETE Inventory Profile Header | [inv_profile_hdr.md](inv_profile_hdr.md#delete-inv-profile-hdrinvProfileHdrUid) |
| GET | /inv-profile-hdr | List Inventory Profile Headers | [inv_profile_hdr.md](inv_profile_hdr.md#get-inv-profile-hdr) |
| POST | /inv-profile-hdr | Create Inventory Profile Header | [inv_profile_hdr.md](inv_profile_hdr.md#post-inv-profile-hdr) |
| POST | /inv-profile-hdr/{customerId}/upload | Upload Excel file to create inventory profile headers | [inv_profile_hdr.md](inv_profile_hdr.md#post-inv-profile-hdrcustomerIdupload) |

### inv_profile_line

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line/{invProfileLineUid} | Get Inventory Profile line Details | [inv_profile_line.md](inv_profile_line.md#get-inv-profile-hdrinvProfileHdrUidinv-profile-lineinvProfileLineUid) |
| PUT | /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line/{invProfileLineUid} | Update Inventory Profile line | [inv_profile_line.md](inv_profile_line.md#put-inv-profile-hdrinvProfileHdrUidinv-profile-lineinvProfileLineUid) |
| DELETE | /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line/{invProfileLineUid} | DELETE Inventory Profile Line | [inv_profile_line.md](inv_profile_line.md#delete-inv-profile-hdrinvProfileHdrUidinv-profile-lineinvProfileLineUid) |
| GET | /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line | List Inventory Profile Lines | [inv_profile_line.md](inv_profile_line.md#get-inv-profile-hdrinvProfileHdrUidinv-profile-line) |
| POST | /inv-profile-hdr/{invProfileHdrUid}/inv-profile-line | Create Inventory Profile Lines | [inv_profile_line.md](inv_profile_line.md#post-inv-profile-hdrinvProfileHdrUidinv-profile-line) |

### inv_warehouse

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /warehouse/{warehouseUid}/adjust | Adjust Inventory | [inv_warehouse.md](inv_warehouse.md#post-warehousewarehouseUidadjust) |
| GET | /warehouse/{warehouseUid}/availability | List inventory availability | [inv_warehouse.md](inv_warehouse.md#get-warehousewarehouseUidavailability) |
| POST | /warehouse/{warehouseUid}/receive | Receive Inventory | [inv_warehouse.md](inv_warehouse.md#post-warehousewarehouseUidreceive) |
| GET | /warehouse/{warehouseUid}/replenish | Get Replenish Information | [inv_warehouse.md](inv_warehouse.md#get-warehousewarehouseUidreplenish) |
| POST | /warehouse/{warehouseUid}/replenish | Replenish Inventory | [inv_warehouse.md](inv_warehouse.md#post-warehousewarehouseUidreplenish) |
| POST | /warehouse/{warehouseUid}/transfer | Transfer Inventory | [inv_warehouse.md](inv_warehouse.md#post-warehousewarehouseUidtransfer) |

### products

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /distributors/{distributorsUid}/products | Create Product | [products.md](products.md#post-distributorsdistributorsUidproducts) |
| GET | /products/{productsUid} | Get Product Details | [products.md](products.md#get-productsproductsUid) |
| PUT | /products/{productsUid} | Update Product | [products.md](products.md#put-productsproductsUid) |
| DELETE | /products/{productsUid} | DELETE Product | [products.md](products.md#delete-productsproductsUid) |
| PUT | /products/{productsUid}/enable | Enable/Disable/Delete Product | [products.md](products.md#put-productsproductsUidenable) |
| GET | /products/find | Find products and items | [products.md](products.md#get-productsfind) |
| GET | /products | List products | [products.md](products.md#get-products) |

### restock_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /restock-hdr/{restockHdrUid} | Get Restock Header Details | [restock_hdr.md](restock_hdr.md#get-restock-hdrrestockHdrUid) |
| PUT | /restock-hdr/{restockHdrUid} | Update Restock Header | [restock_hdr.md](restock_hdr.md#put-restock-hdrrestockHdrUid) |
| DELETE | /restock-hdr/{restockHdrUid} | DELETE Restock Header | [restock_hdr.md](restock_hdr.md#delete-restock-hdrrestockHdrUid) |
| GET | /restock-hdr | List Restock Headers | [restock_hdr.md](restock_hdr.md#get-restock-hdr) |
| POST | /restock-hdr | Create Restock Header | [restock_hdr.md](restock_hdr.md#post-restock-hdr) |

### sections

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /sections/{sectionsUid} | Get section Details | [sections.md](sections.md#get-sectionssectionsUid) |
| PUT | /sections/{sectionsUid} | Update section | [sections.md](sections.md#put-sectionssectionsUid) |
| DELETE | /sections/{sectionsUid} | DELETE section | [sections.md](sections.md#delete-sectionssectionsUid) |
| PUT | /sections/{sectionsUid}/enable | Enable/Disable/Delete section | [sections.md](sections.md#put-sectionssectionsUidenable) |
| GET | /sections | List sections | [sections.md](sections.md#get-sections) |
| POST | /sections | Create section | [sections.md](sections.md#post-sections) |

### usage_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /warehouse/{warehouseUid}/usage | Use Inventory | [usage_hdr.md](usage_hdr.md#post-warehousewarehouseUidusage) |

### warehouse

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /warehouse/{warehouseUid} | Get Warehouse Details | [warehouse.md](warehouse.md#get-warehousewarehouseUid) |
| PUT | /warehouse/{warehouseUid} | Update Warehouse | [warehouse.md](warehouse.md#put-warehousewarehouseUid) |
| DELETE | /warehouse/{warehouseUid} | DELETE Warehouse | [warehouse.md](warehouse.md#delete-warehousewarehouseUid) |
| PUT | /warehouse/{warehouseUid}/enable | Enable/Disable/Delete Warehouse | [warehouse.md](warehouse.md#put-warehousewarehouseUidenable) |
| GET | /warehouse | List Warehouses | [warehouse.md](warehouse.md#get-warehouse) |
| POST | /warehouse | Create Warehouse | [warehouse.md](warehouse.md#post-warehouse) |

### warehouse_x_users

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /warehouse/{warehouseUid}/users/{usersId} | Get Warehouse User Assignment | [warehouse_x_users.md](warehouse_x_users.md#get-warehousewarehouseUidusersusersId) |
| PUT | /warehouse/{warehouseUid}/users/{usersId} | Update Warehouse User Assignment | [warehouse_x_users.md](warehouse_x_users.md#put-warehousewarehouseUidusersusersId) |
| DELETE | /warehouse/{warehouseUid}/users/{usersId} | Remove User from Warehouse (sets status_cd to 700) | [warehouse_x_users.md](warehouse_x_users.md#delete-warehousewarehouseUidusersusersId) |
| GET | /warehouse/{warehouseUid}/users | List Warehouses Users | [warehouse_x_users.md](warehouse_x_users.md#get-warehousewarehouseUidusers) |
| POST | /warehouse/{warehouseUid}/users | Create/Update Warehouse User | [warehouse_x_users.md](warehouse_x_users.md#post-warehousewarehouseUidusers) |
