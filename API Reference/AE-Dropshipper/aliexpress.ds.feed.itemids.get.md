# Fetch items with feedname in simple model

**Path:** `aliexpress.ds.feed.itemids.get`

## Request Parameters

| Name | Type | Required | Description |
|---|---|---|---|
| page_size | Number | No | number of each page |
| category_id | String | No | first level category id, you can get from category query |
| feed_name | String | Yes | query api ‘aliexpress.ds.feedname.get’ |
| search_id | String | No |  |

## Response Parameters

| Name | Type | Description |
|---|---|---|
| result | 4 | result object |
| └ products | 7 | item id list |
| └ search_id | 1 | search id, put it in the next request. Only valid in 1 minutes |
| └ total | 2 | total item id left  |
| rsp_msg | 1 | result msg |
| rsp_code | 2 | result code |
| ret | 3 | true is success, false for fail |
