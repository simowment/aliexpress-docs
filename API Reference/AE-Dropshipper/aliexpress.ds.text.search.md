# text search for ds

**Path:** `aliexpress.ds.text.search`

## Request Parameters

| Name | Type | Required | Description |
|---|---|---|---|
| keyWord | String | No | query word |
| local | String | Yes | lang: en_US |
| countryCode | String | Yes | ship to country |
| categoryId | Number | No | categoryId |
| sortBy | String | No | accept value: min_price,asc min_price,desc orders,asc orders,desc comments,asc comments,desc |
| pageSize | Number | No | page size |
| pageIndex | Number | No | page index |
| currency | String | Yes | currency |
| searchExtend | Object[] | No | search extend |
| └ searchKey | String | No | search key |
| └ searchValue | String | No | search value |
| └ max | String | No | max |
| └ min | String | No | min |
| selectionName | String | No | text search within specific selection |

## Response Parameters

| Name | Type | Description |
|---|---|---|
| code | 1 | code |
| msg | 1 | message |
| data | 4 | data |
| └ totalCount | 2 | total |
| └ pageIndex | 2 | page index |
| └ pageSize | 2 | page size |
| └ products | 9 | products |
| &nbsp;&nbsp;└ salePriceFormat | 1 | sale price |
| &nbsp;&nbsp;└ itemUrl | 1 | item url |
| &nbsp;&nbsp;└ orders | 1 | orders |
| &nbsp;&nbsp;└ score | 1 | score |
| &nbsp;&nbsp;└ title | 1 | title |
| &nbsp;&nbsp;└ itemMainPic | 1 | item main picture url |
| &nbsp;&nbsp;└ cateId | 1 | cateId |
| &nbsp;&nbsp;└ originalPriceFormat | 1 | original price formated |
| &nbsp;&nbsp;└ originMinPrice | 1 | originMinPrice |
| &nbsp;&nbsp;└ itemId | 1 | itemId |
| &nbsp;&nbsp;└ originalPrice | 1 | originalPrice |
| &nbsp;&nbsp;└ originalPriceCurrency | 1 | originalPriceCurrency |
| &nbsp;&nbsp;└ salePrice | 1 | salePrice |
| &nbsp;&nbsp;└ salePriceCurrency | 1 | salePriceCurrency |
| &nbsp;&nbsp;└ targetOriginalPrice | 1 | targetOriginalPrice |
| &nbsp;&nbsp;└ targetOriginalPriceCurrency | 1 | targetOriginalPriceCurrency |
| &nbsp;&nbsp;└ targetSalePrice | 1 | targetSalePrice |
| &nbsp;&nbsp;└ discount | 1 | discount |
| &nbsp;&nbsp;└ productVideoUrl | 1 | product video url |
| &nbsp;&nbsp;└ evaluateRate | 1 | evaluateRate |
| &nbsp;&nbsp;└ type | 1 | "search" for search result, "recommend" for smart recommend engine result |

## Error Codes

| Error Code | Error Description | Solution |
|---|---|---|
| IllegalAccessToken | IllegalAccessToken | AccessToken error, please check the accessToken |
