# AuthApi

All URIs are relative to *https://localhost:8000/api/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**authChangePasswordPost**](AuthApi.md#authChangePasswordPost) | **POST** /auth/change_password | Changes a user&#39;s password.
[**authLoginPost**](AuthApi.md#authLoginPost) | **POST** /auth/login | Logs a user in.
[**authLogoutPost**](AuthApi.md#authLogoutPost) | **POST** /auth/logout | Logs a user out.


<a name="authChangePasswordPost"></a>
# **authChangePasswordPost**
> authChangePasswordPost(inlineObject1)

Changes a user&#39;s password.

    All sessions using the previous password will be logged out.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject1** | [**InlineObject1**](..//Models/InlineObject1.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

[CSRFToken](../README.md#CSRFToken), [OTP](../README.md#OTP), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

<a name="authLoginPost"></a>
# **authLoginPost**
> authLoginPost(inlineObject)

Logs a user in.

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject** | [**InlineObject**](..//Models/InlineObject.md)|  | [optional]

### Return type

null (empty response body)

### Authorization

[CSRFToken](../README.md#CSRFToken)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

<a name="authLogoutPost"></a>
# **authLogoutPost**
> authLogoutPost()

Logs a user out.

### Parameters
This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

