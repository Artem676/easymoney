---
id: convertCurrencyMapToArray
title: convertCurrencyMapToArray
hide_title: true
sidebar_label: convertCurrencyMapToArray
---


# `convertCurrencyMapToArray(CurrencyMap)`

#### Arguments

1. `CurrencyMap` ([CurrencyMap](Description.md#currencymap))

#### Returns

`array` 


**Example**

```ts
import {CurrencyMap, convertCurrencyMapToArray, CurrencyUnitCrypto } from "@easymoney/currency";

const map: CurrencyMap<CurrencyUnitCrypto> = {
    BTC: {code: "BTC", minorUnit: 8, symbol: "BTC"},
    LTC: {code: "LTC", minorUnit: 8, symbol: "LTC"}
}

const array = convertCurrencyMapToArray(map);
// => [{ code: "BTC", minorUnit: 8, symbol: "BTC"},
//     { code: "LTC", minorUnit: 8, symbol: "LTC"}]
```