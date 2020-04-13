# VDart-Challenge - Develop a crypto server as described below

Crypto Server

Please make use of the free API from https://api.hitbtc.com/ to complete this challenge. Create a micro-service with the following endpoint,

GET ```/currency/{symbol}```
Returns the real-time crypto prices of the given currency symbol.
Sample Response:

```
  {
    "id": "ETH",
    "fullName": "Ethereum",
    "ask": "0.054464",
    "bid": "0.054463",
    "last": "0.054463",
    "open": "0.057133",
    "low": "0.053615",
    "high": "0.057559",
    "feeCurrency": "BTC"
}
```
GET ```/currency/all```
Returns the real-time crypto prices of all the supported currencies.
Response: 
```
[
   {
      "id": "BTC",
      "fullName": "Bitcoin",
      "crypto": true,
      "payinEnabled": true,
      "payinPaymentId": false,
      "payinConfirmations": 2,
      "payoutEnabled": true,
      "payoutIsPaymentId": false,
      "transferEnabled": true,
      "delisted": false,
      "payoutFee": "0.00958"
   },
   {
      "id": "ETH",
      "fullName": "Ethereum",
      "crypto": true,
      "payinEnabled": true,
      "payinPaymentId": false,
      "payinConfirmations": 2,
      "payoutEnabled": true,
      "payoutIsPaymentId": false,
      "transferEnabled": true,
      "delisted": false,
      "payoutFee": "0.001"
   }
]
```
