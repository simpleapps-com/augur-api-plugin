---
name: Nexus API
description: Use when working with bin transfer hdr, bin transfer line, health check, purchase order receipt, receiving, seed, transfer, transfer receipt, transfer shipping, users, or making API calls to https://nexus.augur-api.com.
version: 1.0.2
---

# Nexus

Service-specific knowledge for nexus microservice.

## API Documentation

- [OpenAPI Specification](https://nexus.augur-api.com/openapi.json)
- [Postman Collection](https://nexus.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### bin_transfer_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /bin-transfer/{binTransferHdrUid} | Get Bin Transfer Details | [bin_transfer_hdr.md](bin_transfer_hdr.md#get-bin-transferbinTransferHdrUid) |
| PUT | /bin-transfer/{binTransferHdrUid} | Update Bin Transfer | [bin_transfer_hdr.md](bin_transfer_hdr.md#put-bin-transferbinTransferHdrUid) |
| DELETE | /bin-transfer/{binTransferHdrUid} | DELETE Bin Transfer | [bin_transfer_hdr.md](bin_transfer_hdr.md#delete-bin-transferbinTransferHdrUid) |
| GET | /bin-transfer | List Bin Transfers | [bin_transfer_hdr.md](bin_transfer_hdr.md#get-bin-transfer) |
| POST | /bin-transfer | Create Bin Transfer | [bin_transfer_hdr.md](bin_transfer_hdr.md#post-bin-transfer) |
| GET | /bin-transfer/{binTransferHdrUid}/status | Get Bin Transfer Status with Lines | [bin_transfer_hdr.md](bin_transfer_hdr.md#get-bin-transferbinTransferHdrUidstatus) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### purchase_order_receipt

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /purchase-order-receipt/{purchaseOrderReceiptUid} | Get Purchase Order Receipt Details | [purchase_order_receipt.md](purchase_order_receipt.md#get-purchase-order-receiptpurchaseOrderReceiptUid) |
| PUT | /purchase-order-receipt/{purchaseOrderReceiptUid} | Update Purchase Order Receipt | [purchase_order_receipt.md](purchase_order_receipt.md#put-purchase-order-receiptpurchaseOrderReceiptUid) |
| DELETE | /purchase-order-receipt/{purchaseOrderReceiptUid} | DELETE Purchase Order Receipt | [purchase_order_receipt.md](purchase_order_receipt.md#delete-purchase-order-receiptpurchaseOrderReceiptUid) |
| GET | /purchase-order-receipt | List Purchase Order Receipts | [purchase_order_receipt.md](purchase_order_receipt.md#get-purchase-order-receipt) |
| POST | /purchase-order-receipt | Create Purchase Order Receipt | [purchase_order_receipt.md](purchase_order_receipt.md#post-purchase-order-receipt) |

### receiving

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /receiving/{receivingUid} | Get Receiving Details | [receiving.md](receiving.md#get-receivingreceivingUid) |
| PUT | /receiving/{receivingUid} | Update Receiving | [receiving.md](receiving.md#put-receivingreceivingUid) |
| DELETE | /receiving/{receivingUid} | DELETE Receiving | [receiving.md](receiving.md#delete-receivingreceivingUid) |
| GET | /receiving | List Receiving Records | [receiving.md](receiving.md#get-receiving) |
| POST | /receiving | Create Receiving | [receiving.md](receiving.md#post-receiving) |

### transfer

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /transfer/{transferUid} | Get Transfer Details | [transfer.md](transfer.md#get-transfertransferUid) |
| PUT | /transfer/{transferUid} | Update Transfer | [transfer.md](transfer.md#put-transfertransferUid) |
| DELETE | /transfer/{transferUid} | DELETE Transfer | [transfer.md](transfer.md#delete-transfertransferUid) |
| GET | /transfer | List Transfers | [transfer.md](transfer.md#get-transfer) |
| POST | /transfer | Create Transfer | [transfer.md](transfer.md#post-transfer) |

### transfer_receipt

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /transfer-receipt/{transferReceiptUid} | Get Transfer Receipt Details | [transfer_receipt.md](transfer_receipt.md#get-transfer-receipttransferReceiptUid) |
| PUT | /transfer-receipt/{transferReceiptUid} | Update Transfer Receipt | [transfer_receipt.md](transfer_receipt.md#put-transfer-receipttransferReceiptUid) |
| DELETE | /transfer-receipt/{transferReceiptUid} | DELETE Transfer Receipt | [transfer_receipt.md](transfer_receipt.md#delete-transfer-receipttransferReceiptUid) |
| GET | /transfer-receipt | List Transfer Receipts | [transfer_receipt.md](transfer_receipt.md#get-transfer-receipt) |
| POST | /transfer-receipt | Create Transfer Receipt | [transfer_receipt.md](transfer_receipt.md#post-transfer-receipt) |

### transfer_shipping

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /transfer-shipping/{transferReceiptUid} | Get Transfer Shipping Details | [transfer_shipping.md](transfer_shipping.md#get-transfer-shippingtransferReceiptUid) |
| PUT | /transfer-shipping/{transferReceiptUid} | Update Transfer Shipping | [transfer_shipping.md](transfer_shipping.md#put-transfer-shippingtransferReceiptUid) |
| DELETE | /transfer-shipping/{transferReceiptUid} | DELETE Transfer Shipping | [transfer_shipping.md](transfer_shipping.md#delete-transfer-shippingtransferReceiptUid) |
| GET | /transfer-shipping | List Transfer Shippings | [transfer_shipping.md](transfer_shipping.md#get-transfer-shipping) |
| POST | /transfer-shipping | Create Transfer Shipping | [transfer_shipping.md](transfer_shipping.md#post-transfer-shipping) |
