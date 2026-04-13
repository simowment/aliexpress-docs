# API for fetch AE Category's ID and Category Name

**Path:** `aliexpress.ds.category.get`

## Request Parameters

| Name | Type | Required | Description |
|---|---|---|---|
| categoryId | String | No | categoryId |
| language | String | No | language:hi de ru pt ko in en it fr zh es iw ar vi th uk ja id pl he nl tr |
| app_signature | String | No | signature |

## Response Parameters

| Name | Type | Description |
|---|---|---|
| resp_result | 4 |  |
| └ resp_code | 2 |  |
| └ resp_msg | 1 |  |
| └ result | 4 |  |
| &nbsp;&nbsp;└ categories | 9 |  |
| &nbsp;&nbsp;&nbsp;&nbsp;└ category_id | 2 |  |
| &nbsp;&nbsp;&nbsp;&nbsp;└ category_name | 1 |  |
| &nbsp;&nbsp;&nbsp;&nbsp;└ parent_category_id | 2 |  |
| &nbsp;&nbsp;└ total_result_count | 2 |  |

## Error Codes

| Error Code | Error Description | Solution |
|---|---|---|
| UnsupportedParamMapping | UnsupportedParamMapping | Unsupported parameters, please check the parameters |
