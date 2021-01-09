# ExchangeApi

All URIs are relative to *https://localhost:8000/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**exchangeOrdersCancelPost**](ExchangeApi.md#exchangeOrdersCancelPost) | **POST** /exchange/orders/cancel | Cancels a group of orders.
[**exchangeOrdersOrderIdDelete**](ExchangeApi.md#exchangeOrdersOrderIdDelete) | **DELETE** /exchange/orders/{order_id} | Cancels an order by its ID.
[**exchangeOrdersOrderIdGet**](ExchangeApi.md#exchangeOrdersOrderIdGet) | **GET** /exchange/orders/{order_id} | Gets an order by its ID.
[**exchangeOrdersPost**](ExchangeApi.md#exchangeOrdersPost) | **POST** /exchange/orders | Posts an order. Funds will be immediately debited.
[**exchangeOrdersPut**](ExchangeApi.md#exchangeOrdersPut) | **PUT** /exchange/orders | Modifies an existing order. Funds will immediately debited if the quantity increases, or credited if the quantity decreases.


<a name="exchangeOrdersCancelPost"></a>
# **exchangeOrdersCancelPost**
> List exchangeOrdersCancelPost(inlineObject2)

Cancels a group of orders.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject2** | [**InlineObject2**](..//Models/InlineObject2.md)|  |

### Return type

[**List**](..//Models/oneOf&lt;BlockInclusionResponse,BlockInclusionFailure&gt;.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [OTP](../README.md#OTP), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="exchangeOrdersOrderIdDelete"></a>
# **exchangeOrdersOrderIdDelete**
> BlockInclusionResponse exchangeOrdersOrderIdDelete(orderId)

Cancels an order by its ID.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**| Numeric ID of the order. | [default to null]

### Return type

[**BlockInclusionResponse**](..//Models/BlockInclusionResponse.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [OTP](../README.md#OTP), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="exchangeOrdersOrderIdGet"></a>
# **exchangeOrdersOrderIdGet**
> OrderWithFills exchangeOrdersOrderIdGet(orderId)

Gets an order by its ID.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**| Numeric ID of the order. | [default to null]

### Return type

[**OrderWithFills**](..//Models/OrderWithFills.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="exchangeOrdersPost"></a>
# **exchangeOrdersPost**
> OrderCreationResponse exchangeOrdersPost(orderCreationRequest)

Posts an order. Funds will be immediately debited.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderCreationRequest** | [**OrderCreationRequest**](..//Models/OrderCreationRequest.md)|  |

### Return type

[**OrderCreationResponse**](..//Models/OrderCreationResponse.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [OTP](../README.md#OTP), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

<a name="exchangeOrdersPut"></a>
# **exchangeOrdersPut**
> OrderCreationResponse exchangeOrdersPut(order)

Modifies an existing order. Funds will immediately debited if the quantity increases, or credited if the quantity decreases.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **order** | [**Order**](..//Models/Order.md)|  |

### Return type

[**OrderCreationResponse**](..//Models/OrderCreationResponse.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [OTP](../README.md#OTP), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

