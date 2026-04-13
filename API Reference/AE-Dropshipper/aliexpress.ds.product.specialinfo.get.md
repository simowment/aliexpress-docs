# get products' special info like certification

**Path:** `aliexpress.ds.product.specialinfo.get`

## Request Parameters

| Name | Type | Required | Description |
|---|---|---|---|
| itemId | Number | Yes | product id |
| countryCodes | String[] | Yes | country code |
| appKey | String | Yes | your appkey |

## Response Parameters

| Name | Type | Description |
|---|---|---|
| result | 4 | result |
| └ ret | 3 | bool to tag if it is success |
| └ code | 1 | error code  |
| └ data | 4 | data_demo |
| &nbsp;&nbsp;└ product_id | 1 | productId |
| &nbsp;&nbsp;└ item_qualification_list | 9 | item certification list |
| &nbsp;&nbsp;&nbsp;&nbsp;└ value_type | 1 | certification type |
| &nbsp;&nbsp;&nbsp;&nbsp;└ name | 1 | certification name |
| &nbsp;&nbsp;&nbsp;&nbsp;└ value | 1 | certification url |
| &nbsp;&nbsp;&nbsp;&nbsp;└ key | 1 | certification key |
| └ err_message | 1 | error message |
