# Delivery/Freight API

**Path:** `aliexpress.ds.freight.query`

## Request Parameters

| Name | Type | Required | Description |
|---|---|---|---|
| queryDeliveryReq | Object | Yes | delivery query request |
| └ quantity | Number | Yes | quantity for your request |
| └ shipToCountry | String | Yes | country that ships to |
| └ productId | String | Yes | product_id |
| └ provinceCode | String | No | The province code, used to query shipping fees for local-to-local products. Please provide either province or provinceCode; do not provide both. |
| └ cityCode | String | No | The city code. Optional. |
| └ language | String | Yes | language |
| └ locale | String | Yes | locale |
| └ selectedSkuId | String | Yes | selected sku |
| └ currency | String | Yes | currency for calculate the freight fee |
| └ province | String | No | The province name, used to query shipping fees for local-to-local products. Please provide either province or provinceCode; do not provide both. |

## Response Parameters

| Name | Type | Description |
|---|---|---|
| result | 4 | result |
| └ msg | 1 | error msg |
| └ delivery_options | 9 | list of deliveryOptions |
| &nbsp;&nbsp;└ shipping_fee_format | 1 | format String shipping fee to make it understandable |
| &nbsp;&nbsp;└ delivery_date_desc | 1 | format delivery date estimation |
| &nbsp;&nbsp;└ code | 1 | delivery service code, which is used for place order |
| &nbsp;&nbsp;└ free_shipping | 3 | true means free, false means not free |
| &nbsp;&nbsp;└ max_delivery_days | 2 | estimated delivery days, max days |
| &nbsp;&nbsp;└ estimated_delivery_time | 1 | delivery estimation |
| &nbsp;&nbsp;└ min_delivery_days | 2 | estimated delivery days, main days |
| &nbsp;&nbsp;└ shipping_fee_currency | 1 | shipping fee currency |
| &nbsp;&nbsp;└ ship_from_country | 1 | where your sku will ship from |
| &nbsp;&nbsp;└ company | 1 | shipping service company name which you can use to display |
| &nbsp;&nbsp;└ shipping_fee_cent | 1 | shipping fee amount in cent |
| &nbsp;&nbsp;└ tracking | 3 | is this shipping option can be tracking |
| &nbsp;&nbsp;└ mayHavePFS | 3 | if it can be platFormFreeShipping |
| &nbsp;&nbsp;└ available_stock | 1 | available stock for sku |
| &nbsp;&nbsp;└ guaranteed_delivery_days | 1 | it is a guaranteed days |
| &nbsp;&nbsp;└ ddpIncludeVATTax | 1 | if price include ddp vat tax |
| &nbsp;&nbsp;└ free_shipping_threshold | 1 | free shipping threshold |
| └ code | 2 | status of this request: 200 means success |
| └ success | 3 | true means it is success |

## Error Codes

| Error Code | Error Description | Solution |
|---|---|---|
| DELIVERY_NOT_AVAILABLE_TO_YOUR_ADDRESS | DELIVERY_NOT_AVAILABLE_TO_YOUR_ADDRESS | Logistics cannot be delivered to the specified address |
| DELIVERY_INFO_EMPTY | DELIVERY_INFO_EMPTY | The product ID is wrong, please check the product ID |
