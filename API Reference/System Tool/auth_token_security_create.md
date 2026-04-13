# generateSecurityToken

**Path:** `/auth/token/security/create`

## Request Parameters

| Name | Type | Required | Description |
|---|---|---|---|
| code | String | Yes |  |
| uuid | String | No |  |

## Response Parameters

| Name | Type | Description |
|---|---|---|
| expires_in | 2 |  |
| account_id | 1 |  |
| user_id | 1 |  |
| seller_id | 1 |  |
| access_token | 1 |  |
| refresh_token | 1 |  |
| refresh_expires_in | 2 |  |
| expire_time | 2 |  |
| refresh_token_valid_time | 2 |  |
| sp | 1 |  |
| locale | 1 |  |

## Error Codes

| Error Code | Error Description | Solution |
|---|---|---|
| isv.402 | Creation failed | Parameter error, please check the parameters |
