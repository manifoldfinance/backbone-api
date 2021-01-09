# Documentation for Manifold REST API

<a name="documentation-for-api-endpoints"></a>
## Documentation for API Endpoints

All URIs are relative to *https://localhost:8000/api/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AuthApi* | [**authChangePasswordPost**](Apis/AuthApi.md#authchangepasswordpost) | **POST** /auth/change_password | Changes a user's password.
*AuthApi* | [**authLoginPost**](Apis/AuthApi.md#authloginpost) | **POST** /auth/login | Logs a user in.
*AuthApi* | [**authLogoutPost**](Apis/AuthApi.md#authlogoutpost) | **POST** /auth/logout | Logs a user out.
*ExchangeApi* | [**exchangeOrdersCancelPost**](Apis/ExchangeApi.md#exchangeorderscancelpost) | **POST** /exchange/orders/cancel | Cancels a group of orders.
*ExchangeApi* | [**exchangeOrdersOrderIdDelete**](Apis/ExchangeApi.md#exchangeordersorderiddelete) | **DELETE** /exchange/orders/{order_id} | Cancels an order by its ID.
*ExchangeApi* | [**exchangeOrdersOrderIdGet**](Apis/ExchangeApi.md#exchangeordersorderidget) | **GET** /exchange/orders/{order_id} | Gets an order by its ID.
*ExchangeApi* | [**exchangeOrdersPost**](Apis/ExchangeApi.md#exchangeorderspost) | **POST** /exchange/orders | Posts an order. Funds will be immediately debited.
*ExchangeApi* | [**exchangeOrdersPut**](Apis/ExchangeApi.md#exchangeordersput) | **PUT** /exchange/orders | Modifies an existing order. Funds will immediately debited if the quantity increases, or credited if the quantity decreases.
*MarketApi* | [**marketsGet**](Apis/MarketApi.md#marketsget) | **GET** /markets | Lists all markets.
*MarketApi* | [**marketsMarketIdBatchesBlockNumberGet**](Apis/MarketApi.md#marketsmarketidbatchesblocknumberget) | **GET** /markets/{market_id}/batches/{block_number} | Gets all executed batches at a block (or latest)
*MarketApi* | [**marketsMarketIdBookGet**](Apis/MarketApi.md#marketsmarketidbookget) | **GET** /markets/{market_id}/book | Gets all open order at latest block by market
*MarketApi* | [**marketsMarketIdCandlesGet**](Apis/MarketApi.md#marketsmarketidcandlesget) | **GET** /markets/{market_id}/candles | Gets candlestick prices for the provided market.
*MarketApi* | [**marketsMarketIdDailyGet**](Apis/MarketApi.md#marketsmarketiddailyget) | **GET** /markets/{market_id}/daily | Daily Price Stats
*MarketApi* | [**marketsMarketIdSpreadBlockNumberGet**](Apis/MarketApi.md#marketsmarketidspreadblocknumberget) | **GET** /markets/{market_id}/spread/{block_number} | Gets the batch auction state for the provided market ID and the block number.
*UserApi* | [**userBalanceGet**](Apis/UserApi.md#userbalanceget) | **GET** /user/balance | Returns the user's balance across all supported chains.
*UserApi* | [**userDepositsPost**](Apis/UserApi.md#userdepositspost) | **POST** /user/deposits | Registers a MEV deposit on the YCabal.
*UserApi* | [**userFillsGet**](Apis/UserApi.md#userfillsget) | **GET** /user/fills | Gets all fills relevant to this user.
*UserApi* | [**userOrdersGet**](Apis/UserApi.md#userordersget) | **GET** /user/orders | Gets all orders created by this user.
*UserApi* | [**userSendPost**](Apis/UserApi.md#usersendpost) | **POST** /user/send | Transfers Funds
*UserApi* | [**userWithdrawalsGet**](Apis/UserApi.md#userwithdrawalsget) | **GET** /user/withdrawals | Gets the user's list of withdrawals.
*UserApi* | [**userWithdrawalsPost**](Apis/UserApi.md#userwithdrawalspost) | **POST** /user/withdrawals | Initiates a withdrawal of a cleared asset.


<a name="documentation-for-models"></a>
## Documentation for Models

 - [Balance](.//Models/Balance.md)
 - [BalanceBalances](.//Models/BalanceBalances.md)
 - [BatchInfo](.//Models/BatchInfo.md)
 - [BatchesResponse](.//Models/BatchesResponse.md)
 - [BlockInclusionFailure](.//Models/BlockInclusionFailure.md)
 - [BlockInclusionFailureError](.//Models/BlockInclusionFailureError.md)
 - [BlockInclusionResponse](.//Models/BlockInclusionResponse.md)
 - [BlockInclusionResponseBlockInclusion](.//Models/BlockInclusionResponseBlockInclusion.md)
 - [CandlestickResponse](.//Models/CandlestickResponse.md)
 - [CandlestickResponseCandles](.//Models/CandlestickResponseCandles.md)
 - [Fill](.//Models/Fill.md)
 - [InlineObject](.//Models/InlineObject.md)
 - [InlineObject1](.//Models/InlineObject1.md)
 - [InlineObject2](.//Models/InlineObject2.md)
 - [InlineObject3](.//Models/InlineObject3.md)
 - [InlineObject4](.//Models/InlineObject4.md)
 - [InlineObject5](.//Models/InlineObject5.md)
 - [InlineResponse200](.//Models/InlineResponse200.md)
 - [InlineResponse2001](.//Models/InlineResponse2001.md)
 - [InlineResponse2002](.//Models/InlineResponse2002.md)
 - [InlineResponse2003](.//Models/InlineResponse2003.md)
 - [Market](.//Models/Market.md)
 - [Order](.//Models/Order.md)
 - [OrderCreationRequest](.//Models/OrderCreationRequest.md)
 - [OrderCreationResponse](.//Models/OrderCreationResponse.md)
 - [OrderWithFills](.//Models/OrderWithFills.md)
 - [PriceQuantity](.//Models/PriceQuantity.md)
 - [Spread](.//Models/Spread.md)
 - [Withdrawal](.//Models/Withdrawal.md)


<a name="documentation-for-authorization"></a>
## Documentation for Authorization

<a name="CSRFToken"></a>
### CSRFToken

- **Type**: API key
- **API key parameter name**: X-CSRF-Token
- **Location**: HTTP header

<a name="OTP"></a>
### OTP

- **Type**: API key
- **API key parameter name**: X-OTP-Token
- **Location**: HTTP header

<a name="SessionCookie"></a>
### SessionCookie

- **Type**: API key
- **API key parameter name**: uex_session
- **Location**: 

