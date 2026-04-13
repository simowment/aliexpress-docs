# refreshToken

**Path:** `/auth/token/refresh`

## Request Parameters

| Name | Type | Required | Description |
|---|---|---|---|
| refresh_token | String | Yes |  |

## Response Parameters

| Name | Type | Description |
|---|---|---|
| expires_in | 2 |  |
| account_id | 1 |  |
| seller_id | 1 |  |
| user_id | 1 |  |
| user_nick | 1 |  |
| havana_id | 1 |  |
| account_platform | 1 |  |
| access_token | 1 |  |
| account | 1 |  |
| refresh_token | 1 |  |
| refresh_expires_in | 2 |  |
| expire_time | 2 |  |
| refresh_token_valid_time | 2 |  |
| sp | 1 |  |
| locale | 1 |  |

## Error Codes

| Error Code | Error Description | Solution |
|---|---|---|
| IllegalRefreshToken | Illegal Refresh Token | The specified refresh token is invalid or expired, please check and try again |
| AUTH_TYPE_UNSUPPORTED | Authorization type not supported | The authorization type is not supported. Please check the authorization type. |
| IllegalAccessToken | Illegal Access Token | The access token is invalid, please check and try again |
