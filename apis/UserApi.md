# UserApi

All URIs are relative to _https://localhost:8000/api/v1_

| Method                                                    | HTTP request               | Description                                                 |
| --------------------------------------------------------- | -------------------------- | ----------------------------------------------------------- |
| [**userBalanceGet**](UserApi.md#userBalanceGet)           | **GET** /user/balance      | Returns the user&#39;s balance across all supported chains. |
| [**userDepositsPost**](UserApi.md#userDepositsPost)       | **POST** /user/deposits    | Registers a MEV deposit on the YCabal.                      |
| [**userFillsGet**](UserApi.md#userFillsGet)               | **GET** /user/fills        | Gets all fills relevant to this user.                       |
| [**userOrdersGet**](UserApi.md#userOrdersGet)             | **GET** /user/orders       | Gets all orders created by this user.                       |
| [**userSendPost**](UserApi.md#userSendPost)               | **POST** /user/send        | Transfers Funds                                             |
| [**userWithdrawalsGet**](UserApi.md#userWithdrawalsGet)   | **GET** /user/withdrawals  | Gets the user&#39;s list of withdrawals.                    |
| [**userWithdrawalsPost**](UserApi.md#userWithdrawalsPost) | **POST** /user/withdrawals | Initiates a withdrawal of a cleared asset.                  |

<a name="userBalanceGet"></a>

# **userBalanceGet**

> Balance userBalanceGet()

Returns the user&#39;s balance across all supported chains.

### Parameters

This endpoint does not need any parameter.

### Return type

[**Balance**](..//Models/Balance.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="userDepositsPost"></a>

# **userDepositsPost**

> BlockInclusionResponse userDepositsPost(inlineObject5)

Registers a MEV deposit on the YCabal.

### Parameters

| Name              | Type                                             | Description | Notes |
| ----------------- | ------------------------------------------------ | ----------- | ----- |
| **inlineObject5** | [**InlineObject5**](..//Models/InlineObject5.md) |             |

### Return type

[**BlockInclusionResponse**](..//Models/BlockInclusionResponse.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="userFillsGet"></a>

# **userFillsGet**

> inline_response_200_1 userFillsGet(startBlock, endBlock)

Gets all fills relevant to this user.

### Parameters

| Name           | Type        | Description                       | Notes                       |
| -------------- | ----------- | --------------------------------- | --------------------------- |
| **startBlock** | **Integer** | The block to start counting from. | [optional][default to null] |
| **endBlock**   | **Integer** | The block to end counting at.     | [optional][default to null] |

### Return type

[**inline_response_200_1**](..//Models/inline_response_200_1.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="userOrdersGet"></a>

# **userOrdersGet**

> inline_response_200 userOrdersGet(start)

Gets all orders created by this user.

### Parameters

| Name      | Type        | Description                  | Notes                       |
| --------- | ----------- | ---------------------------- | --------------------------- |
| **start** | **Integer** | The ID to begin counting at. | [optional][default to null] |

### Return type

[**inline_response_200**](..//Models/inline_response_200.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="userSendPost"></a>

# **userSendPost**

> BlockInclusionResponse userSendPost(inlineObject3)

Transfers Funds

### Parameters

| Name              | Type                                             | Description | Notes |
| ----------------- | ------------------------------------------------ | ----------- | ----- |
| **inlineObject3** | [**InlineObject3**](..//Models/InlineObject3.md) |             |

### Return type

[**BlockInclusionResponse**](..//Models/BlockInclusionResponse.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="userWithdrawalsGet"></a>

# **userWithdrawalsGet**

> inline_response_200_2 userWithdrawalsGet()

Gets the user&#39;s list of withdrawals.

### Parameters

This endpoint does not need any parameter.

### Return type

[**inline_response_200_2**](..//Models/inline_response_200_2.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="userWithdrawalsPost"></a>

# **userWithdrawalsPost**

> Withdrawal userWithdrawalsPost(inlineObject4)

Initiates a withdrawal of a cleared asset.

### Parameters

| Name              | Type                                             | Description | Notes |
| ----------------- | ------------------------------------------------ | ----------- | ----- |
| **inlineObject4** | [**InlineObject4**](..//Models/InlineObject4.md) |             |

### Return type

[**Withdrawal**](..//Models/Withdrawal.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json
