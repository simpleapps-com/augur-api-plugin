---
name: Items API
description: Use when working with alternate code, assembly hdr, assembly line, attribute, attribute group, attribute group x attribute value, attribute value, attribute x attribute group, bin, brands, brands x items, categories, contracts items, data type context, health check, internal, inv accessory, inv adj hdr, inv bin, inv loc, inv loc stock status, inv mast, inv mast 15, inv mast attributes, inv mast context, inv mast external, inv mast faq, inv mast language, inv mast links, inv mast lot, inv mast msds, inv mast similarity hdr, inv mast similarity line, inv mast sub parts, inv mast ud, inv mast x restricted class, inv period usage, inv sub, inv xref, inventory receipts hdr, inventory supplier, inventory supplier x loc, item attribute value, item catalog, item catalog def, item catalog def detail, item category, item category hierarchy, item category hierarchy delete audit, item category image, item category link, item category meaning, item category text, item category ud, item category x inv mast, item conversion, item favorites, item meaning, item metrics, item package type, item price hash, item uom, item variant hdr, item variant line, item wishlist hdr, item wishlist line, package type, promotional group det, promotional group hdr, refresh items log, seed, sync tracking hdr, sync tracking line, unit of measure, web display type, or making API calls to https://items.augur-api.com.
version: 1.0.3
---

# Items

Service-specific knowledge for items microservice.

## API Documentation

- [OpenAPI Specification](https://items.augur-api.com/openapi.json)
- [Postman Collection](https://items.augur-api.com/postman.json)

## Authentication

All endpoints except `/health-check` and `/ping` require bearer token authentication. See [authentication.md](../augur-api/authentication.md) for details.

## API Endpoints

### alternate_code

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/alternate-code | List alternate codes | [alternate_code.md](alternate_code.md#get-inv-mastinvMastUidalternate-code) |

### attribute

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /attributes/{attributeUid} | Get Attribute Group Details | [attribute.md](attribute.md#get-attributesattributeUid) |
| PUT | /attributes/{attributeUid} | Update Attribute | [attribute.md](attribute.md#put-attributesattributeUid) |
| DELETE | /attributes/{attributeUid} | DELETE Attribute | [attribute.md](attribute.md#delete-attributesattributeUid) |
| GET | /attributes | List Attributes | [attribute.md](attribute.md#get-attributes) |
| POST | /attributes | Create Attribute | [attribute.md](attribute.md#post-attributes) |

### attribute_group

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /attribute-groups/{attributeGroupUid} | Get Attribute Group Details | [attribute_group.md](attribute_group.md#get-attribute-groupsattributeGroupUid) |
| PUT | /attribute-groups/{attributeGroupUid} | Update Attribute Group | [attribute_group.md](attribute_group.md#put-attribute-groupsattributeGroupUid) |
| DELETE | /attribute-groups/{attributeGroupUid} | DELETE Attribute Group | [attribute_group.md](attribute_group.md#delete-attribute-groupsattributeGroupUid) |
| GET | /attribute-groups | List Attribute Groups | [attribute_group.md](attribute_group.md#get-attribute-groups) |
| POST | /attribute-groups | Create Attribute Group | [attribute_group.md](attribute_group.md#post-attribute-groups) |

### attribute_value

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /attributes/{attributeUid}/values/{attributeValueUid} | Get AttributeValue Details | [attribute_value.md](attribute_value.md#get-attributesattributeUidvaluesattributeValueUid) |
| PUT | /attributes/{attributeUid}/values/{attributeValueUid} | Update AttributeValue | [attribute_value.md](attribute_value.md#put-attributesattributeUidvaluesattributeValueUid) |
| DELETE | /attributes/{attributeUid}/values/{attributeValueUid} | DELETE AttributeValue | [attribute_value.md](attribute_value.md#delete-attributesattributeUidvaluesattributeValueUid) |
| GET | /attributes/{attributeUid}/values | List AttributeValues | [attribute_value.md](attribute_value.md#get-attributesattributeUidvalues) |
| POST | /attributes/{attributeUid}/values | Create AttributeValue | [attribute_value.md](attribute_value.md#post-attributesattributeUidvalues) |

### attribute_x_attribute_group

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /attribute-groups/{attributeGroupUid}/attributes/{attributeXAttributeGroupUid} | Get Attribute X Attribute Group Details | [attribute_x_attribute_group.md](attribute_x_attribute_group.md#get-attribute-groupsattributeGroupUidattributesattributeXAttributeGroupUid) |
| PUT | /attribute-groups/{attributeGroupUid}/attributes/{attributeXAttributeGroupUid} | Update Attribute X Attribute Group | [attribute_x_attribute_group.md](attribute_x_attribute_group.md#put-attribute-groupsattributeGroupUidattributesattributeXAttributeGroupUid) |
| DELETE | /attribute-groups/{attributeGroupUid}/attributes/{attributeXAttributeGroupUid} | DELETE Attribute X Attribute Group | [attribute_x_attribute_group.md](attribute_x_attribute_group.md#delete-attribute-groupsattributeGroupUidattributesattributeXAttributeGroupUid) |
| GET | /attribute-groups/{attributeGroupUid}/attributes | List Attribute X Attribute Groups | [attribute_x_attribute_group.md](attribute_x_attribute_group.md#get-attribute-groupsattributeGroupUidattributes) |
| POST | /attribute-groups/{attributeGroupUid}/attributes | Create Attribute X Attribute Group | [attribute_x_attribute_group.md](attribute_x_attribute_group.md#post-attribute-groupsattributeGroupUidattributes) |

### brands

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /brands/{brandsUid} | Get Brands Details | [brands.md](brands.md#get-brandsbrandsUid) |
| PUT | /brands/{brandsUid} | Update Brands | [brands.md](brands.md#put-brandsbrandsUid) |
| DELETE | /brands/{brandsUid} | DELETE Brands | [brands.md](brands.md#delete-brandsbrandsUid) |
| GET | /brands | List Brands | [brands.md](brands.md#get-brands) |
| POST | /brands | Create Brands | [brands.md](brands.md#post-brands) |

### brands_x_items

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /brands/{brandsUid}/items/{brandsXItemsUid} | Get Brands X Items Details | [brands_x_items.md](brands_x_items.md#get-brandsbrandsUiditemsbrandsXItemsUid) |
| PUT | /brands/{brandsUid}/items/{brandsXItemsUid} | Update Brands X Items | [brands_x_items.md](brands_x_items.md#put-brandsbrandsUiditemsbrandsXItemsUid) |
| DELETE | /brands/{brandsUid}/items/{brandsXItemsUid} | DELETE Brands X Items | [brands_x_items.md](brands_x_items.md#delete-brandsbrandsUiditemsbrandsXItemsUid) |
| GET | /brands/{brandsUid}/items | List Brands X Items | [brands_x_items.md](brands_x_items.md#get-brandsbrandsUiditems) |
| POST | /brands/{brandsUid}/items | Create Brands X Items | [brands_x_items.md](brands_x_items.md#post-brandsbrandsUiditems) |

### categories

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /categories/{itemCategoryUid}/attributes | list the attributes in a category | [categories.md](categories.md#get-categoriesitemCategoryUidattributes) |
| GET | /categories/{itemCategoryUid} | Get the category details | [categories.md](categories.md#get-categoriesitemCategoryUid) |
| GET | /categories/{itemCategoryUid}/images | list the images for a category | [categories.md](categories.md#get-categoriesitemCategoryUidimages) |
| GET | /categories/{itemCategoryUid}/items | list the items in a category | [categories.md](categories.md#get-categoriesitemCategoryUiditems) |
| GET | /categories/lookup | lookup the categories details | [categories.md](categories.md#get-categorieslookup) |

### contracts_items

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /contracts/{jobNo}/attributes | list the attributes for contract items | [contracts_items.md](contracts_items.md#get-contractsjobNoattributes) |
| GET | /contracts/{jobNo}/items | List contracts items for a job | [contracts_items.md](contracts_items.md#get-contractsjobNoitems) |

### health_check

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /health-check | Health Check | [health_check.md](health_check.md#get-health-check) |
| GET | /ping | Ping to get Pong | [health_check.md](health_check.md#get-ping) |

### internal

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| POST | /internal/pdf | Generate PDF | [internal.md](internal.md#post-internalpdf) |

### inv_accessory

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/inv-accessory | List accessory items | [inv_accessory.md](inv_accessory.md#get-inv-mastinvMastUidinv-accessory) |

### inv_bin

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/locations/{locationId}/bins/{bin} | Get a specific bin for an inventory item at a specific location | [inv_bin.md](inv_bin.md#get-inv-mastinvMastUidlocationslocationIdbinsbin) |
| GET | /inv-mast/{invMastUid}/locations/{locationId}/bins | List bins for a specific location | [inv_bin.md](inv_bin.md#get-inv-mastinvMastUidlocationslocationIdbins) |
| GET | /locations/{locationId}/bins/{bin} | List all items in a specific bin | [inv_bin.md](inv_bin.md#get-locationslocationIdbinsbin) |
| GET | /locations/{locationId}/bins | List all items in bins at a location | [inv_bin.md](inv_bin.md#get-locationslocationIdbins) |

### inv_loc

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-loc | List InvLoc | [inv_loc.md](inv_loc.md#get-inv-loc) |
| GET | /inv-mast/{invMastUid}/stock | get the inv_mast stock | [inv_loc.md](inv_loc.md#get-inv-mastinvMastUidstock) |

### inv_mast

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid} | get the inv_mast details | [inv_mast.md](inv_mast.md#get-inv-mastinvMastUid) |
| GET | /inv-mast/lookup | Lookup InvMast by search query | [inv_mast.md](inv_mast.md#get-inv-mastlookup) |
| GET | /inv-mast | List InvMast | [inv_mast.md](inv_mast.md#get-inv-mast) |
| GET | /inv-mast/{invMastUid}/doc | get the inv_mast document | [inv_mast.md](inv_mast.md#get-inv-mastinvMastUiddoc) |
| GET | /p21/inv-mast | List raw inv_mast P21 data | [inv_mast.md](inv_mast.md#get-p21inv-mast) |

### inv_mast_faq

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/faq/{invMastFaqUid} | Get Item FAQ Details | [inv_mast_faq.md](inv_mast_faq.md#get-inv-mastinvMastUidfaqinvMastFaqUid) |
| PUT | /inv-mast/{invMastUid}/faq/{invMastFaqUid} | Update Item FAQ | [inv_mast_faq.md](inv_mast_faq.md#put-inv-mastinvMastUidfaqinvMastFaqUid) |
| DELETE | /inv-mast/{invMastUid}/faq/{invMastFaqUid} | DELETE Item FAQ | [inv_mast_faq.md](inv_mast_faq.md#delete-inv-mastinvMastUidfaqinvMastFaqUid) |
| GET | /inv-mast/{invMastUid}/faq | List Item FAQs | [inv_mast_faq.md](inv_mast_faq.md#get-inv-mastinvMastUidfaq) |
| POST | /inv-mast/{invMastUid}/faq | Create Item FAQ | [inv_mast_faq.md](inv_mast_faq.md#post-inv-mastinvMastUidfaq) |

### inv_mast_links

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast-links/{invMastUid} | List document links for an item | [inv_mast_links.md](inv_mast_links.md#get-inv-mast-linksinvMastUid) |

### inv_mast_similarity_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/similar | List similar items | [inv_mast_similarity_hdr.md](inv_mast_similarity_hdr.md#get-inv-mastinvMastUidsimilar) |

### inv_mast_sub_parts

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast-sub-parts/{invMastUid} | List sub parts for an item | [inv_mast_sub_parts.md](inv_mast_sub_parts.md#get-inv-mast-sub-partsinvMastUid) |

### inv_mast_ud

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast-ud | List inv_mast_ud records with filtering and pagination | [inv_mast_ud.md](inv_mast_ud.md#get-inv-mast-ud) |

### inv_sub

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /inv-mast/{invMastUid}/inv-sub | List substitute items | [inv_sub.md](inv_sub.md#get-inv-mastinvMastUidinv-sub) |

### item_attribute_value

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| PUT | /inv-mast/{invMastUid}/attributes/{attributeUid}/values/{attributeValueUid} | Update the status of an attribute value | [item_attribute_value.md](item_attribute_value.md#put-inv-mastinvMastUidattributesattributeUidvaluesattributeValueUid) |
| DELETE | /inv-mast/{invMastUid}/attributes/{attributeUid}/values/{attributeValueUid} | Soft delete an attribute value | [item_attribute_value.md](item_attribute_value.md#delete-inv-mastinvMastUidattributesattributeUidvaluesattributeValueUid) |
| GET | /inv-mast/{invMastUid}/attributes/{attributeUid}/values | List values for a specific item attribute | [item_attribute_value.md](item_attribute_value.md#get-inv-mastinvMastUidattributesattributeUidvalues) |
| POST | /inv-mast/{invMastUid}/attributes/{attributeUid}/values | Create a new attribute value for an item using a specific attribute | [item_attribute_value.md](item_attribute_value.md#post-inv-mastinvMastUidattributesattributeUidvalues) |
| GET | /inv-mast/{invMastUid}/attributes | List item attributes | [item_attribute_value.md](item_attribute_value.md#get-inv-mastinvMastUidattributes) |
| POST | /inv-mast/{invMastUid}/attributes | Create a new attribute value for an item | [item_attribute_value.md](item_attribute_value.md#post-inv-mastinvMastUidattributes) |

### item_category

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-category/{itemCategoryUid} | get the item_category details | [item_category.md](item_category.md#get-item-categoryitemCategoryUid) |
| GET | /item-category/lookup | lookup the item_category details | [item_category.md](item_category.md#get-item-categorylookup) |
| GET | /item-category | list of categories | [item_category.md](item_category.md#get-item-category) |
| GET | /item-category/{itemCategoryUid}/doc | get the item_category document | [item_category.md](item_category.md#get-item-categoryitemCategoryUiddoc) |

### item_favorites

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-favorites/{usersId} | List the item favorites for a user | [item_favorites.md](item_favorites.md#get-item-favoritesusersId) |
| POST | /item-favorites/{usersId} | Create a new item favorite | [item_favorites.md](item_favorites.md#post-item-favoritesusersId) |
| PUT | /item-favorites/{usersId}/{invMastUid} | Update an item favorite | [item_favorites.md](item_favorites.md#put-item-favoritesusersIdinvMastUid) |
| DELETE | /item-favorites/{usersId}/{invMastUid} | Soft Delete an item from a user's favorites | [item_favorites.md](item_favorites.md#delete-item-favoritesusersIdinvMastUid) |

### item_uom

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-uom/{itemUomUid} | Get Item UOM Details | [item_uom.md](item_uom.md#get-item-uomitemUomUid) |
| GET | /item-uom | List Item UOMs | [item_uom.md](item_uom.md#get-item-uom) |

### item_variant_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /variants/{itemVariantHdrUid} | Get Item Variant Header Details | [item_variant_hdr.md](item_variant_hdr.md#get-variantsitemVariantHdrUid) |
| PUT | /variants/{itemVariantHdrUid} | Update Item Variant Header | [item_variant_hdr.md](item_variant_hdr.md#put-variantsitemVariantHdrUid) |
| DELETE | /variants/{itemVariantHdrUid} | DELETE Item Variant Header | [item_variant_hdr.md](item_variant_hdr.md#delete-variantsitemVariantHdrUid) |
| GET | /variants | List Item Variant Headers | [item_variant_hdr.md](item_variant_hdr.md#get-variants) |
| POST | /variants | Create Item Variant Header | [item_variant_hdr.md](item_variant_hdr.md#post-variants) |

### item_variant_line

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /variants/{itemVariantHdrUid}/lines/{itemVariantLineUid} | Get Item Variant Line Details | [item_variant_line.md](item_variant_line.md#get-variantsitemVariantHdrUidlinesitemVariantLineUid) |
| PUT | /variants/{itemVariantHdrUid}/lines/{itemVariantLineUid} | Update Item Variant Line | [item_variant_line.md](item_variant_line.md#put-variantsitemVariantHdrUidlinesitemVariantLineUid) |
| DELETE | /variants/{itemVariantHdrUid}/lines/{itemVariantLineUid} | DELETE Item Variant Line | [item_variant_line.md](item_variant_line.md#delete-variantsitemVariantHdrUidlinesitemVariantLineUid) |
| GET | /variants/{itemVariantHdrUid}/lines | List Item Variant Lines | [item_variant_line.md](item_variant_line.md#get-variantsitemVariantHdrUidlines) |
| POST | /variants/{itemVariantHdrUid}/lines | Create Item Variant Line | [item_variant_line.md](item_variant_line.md#post-variantsitemVariantHdrUidlines) |

### item_wishlist_hdr

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-wishlist/{usersId} | List the item wishlists for a user | [item_wishlist_hdr.md](item_wishlist_hdr.md#get-item-wishlistusersId) |
| POST | /item-wishlist/{usersId} | Create a new item wishlist | [item_wishlist_hdr.md](item_wishlist_hdr.md#post-item-wishlistusersId) |
| PUT | /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid} | Update a new item wishlist | [item_wishlist_hdr.md](item_wishlist_hdr.md#put-item-wishlistusersIdhdritemWishlistHdrUid) |
| DELETE | /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid} | Delete an item wishlist | [item_wishlist_hdr.md](item_wishlist_hdr.md#delete-item-wishlistusersIdhdritemWishlistHdrUid) |

### item_wishlist_line

| Method | Endpoint | Description | Details |
|--------|----------|-------------|---------|
| GET | /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid} | List items in a wishlist | [item_wishlist_line.md](item_wishlist_line.md#get-item-wishlistusersIdhdritemWishlistHdrUid) |
| POST | /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid} | Create one more more item in a wishlist | [item_wishlist_line.md](item_wishlist_line.md#post-item-wishlistusersIdhdritemWishlistHdrUid) |
| DELETE | /item-wishlist/{usersId}/hdr/{itemWishlistHdrUid}/line/{itemWishlistLineUid} | Delete an item from a wishlist | [item_wishlist_line.md](item_wishlist_line.md#delete-item-wishlistusersIdhdritemWishlistHdrUidlineitemWishlistLineUid) |
