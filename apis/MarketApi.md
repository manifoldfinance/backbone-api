# MarketApi

All URIs are relative to _https://localhost:8000/api/v1_

| Method                                                                                        | HTTP request                                        | Description                                                                   |
| --------------------------------------------------------------------------------------------- | --------------------------------------------------- | ----------------------------------------------------------------------------- |
| [**marketsGet**](MarketApi.md#marketsGet)                                                     | **GET** /markets                                    | Lists all markets.                                                            |
| [**marketsMarketIdBatchesBlockNumberGet**](MarketApi.md#marketsMarketIdBatchesBlockNumberGet) | **GET** /markets/{market_id}/batches/{block_number} | Gets all executed batches at a block (or latest)                              |
| [**marketsMarketIdBookGet**](MarketApi.md#marketsMarketIdBookGet)                             | **GET** /markets/{market_id}/book                   | Gets all open order at latest block by market                                 |
| [**marketsMarketIdCandlesGet**](MarketApi.md#marketsMarketIdCandlesGet)                       | **GET** /markets/{market_id}/candles                | Gets candlestick prices for the provided market.                              |
| [**marketsMarketIdDailyGet**](MarketApi.md#marketsMarketIdDailyGet)                           | **GET** /markets/{market_id}/daily                  | Daily Price Stats                                                             |
| [**marketsMarketIdSpreadBlockNumberGet**](MarketApi.md#marketsMarketIdSpreadBlockNumberGet)   | **GET** /markets/{market_id}/spread/{block_number}  | Gets the batch auction state for the provided market ID and the block number. |

<a name="marketsGet"></a>

# **marketsGet**

> Market marketsGet()

Lists all markets.

### Parameters

This endpoint does not need any parameter.

### Return type

[**Market**](..//Models/Market.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="marketsMarketIdBatchesBlockNumberGet"></a>

# **marketsMarketIdBatchesBlockNumberGet**

> BatchesResponse marketsMarketIdBatchesBlockNumberGet(marketId, blockNumber)

Gets all executed batches at a block (or latest)

### Parameters

| Name            | Type       | Description | Notes             |
| --------------- | ---------- | ----------- | ----------------- |
| **marketId**    | **String** |             | [default to null] |
| **blockNumber** | **String** |             | [default to null] |

### Return type

[**BatchesResponse**](..//Models/BatchesResponse.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="marketsMarketIdBookGet"></a>

# **marketsMarketIdBookGet**

> Spread marketsMarketIdBookGet(marketId)

Gets all open order at latest block by market

### Parameters

| Name         | Type       | Description | Notes             |
| ------------ | ---------- | ----------- | ----------------- |
| **marketId** | **String** |             | [default to null] |

### Return type

[**Spread**](..//Models/Spread.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="marketsMarketIdCandlesGet"></a>

# **marketsMarketIdCandlesGet**

> CandlestickResponse marketsMarketIdCandlesGet(marketId, start, end, granularity)

Gets candlestick prices for the provided market.

### Parameters

| Name            | Type       | Description                                     | Notes                                                    |
| --------------- | ---------- | ----------------------------------------------- | -------------------------------------------------------- |
| **marketId**    | **String** | The ID of the market to fetch candles for.      | [default to null]                                        |
| **start**       | **String** | ISO8601 date of when to start the candle query. | [optional][default to null]                              |
| **end**         | **String** | ISO8601 date of when to end the candle query.   | [optional][default to null]                              |
| **granularity** | **String** | Granularity of candle data to return.           | [optional][default to null] [enum: 1m, 5m, 15m, 60m, 1d] |

### Return type

[**CandlestickResponse**](..//Models/CandlestickResponse.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="marketsMarketIdDailyGet"></a>

# **marketsMarketIdDailyGet**

> inline_response_200_3 marketsMarketIdDailyGet(marketId)

Daily Price Stats

### Parameters

| Name         | Type       | Description | Notes             |
| ------------ | ---------- | ----------- | ----------------- |
| **marketId** | **String** |             | [default to null] |

### Return type

[**inline_response_200_3**](..//Models/inline_response_200_3.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

<a name="marketsMarketIdSpreadBlockNumberGet"></a>

# **marketsMarketIdSpreadBlockNumberGet**

> Spread marketsMarketIdSpreadBlockNumberGet(marketId, blockNumber)

Gets the batch auction state for the provided market ID and the block number.

### Parameters

| Name            | Type       | Description | Notes             |
| --------------- | ---------- | ----------- | ----------------- |
| **marketId**    | **String** |             | [default to null] |
| **blockNumber** | **String** |             | [default to null] |

### Return type

[**Spread**](..//Models/Spread.md)

### Authorization

[CSRFToken](../README.md#CSRFToken), [SessionCookie](../README.md#SessionCookie)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json
