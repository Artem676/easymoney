---
id: format
title: format
hide_title: true
sidebar_label: format
---


# `format(money,locale?,options?)`

#### Arguments

1. `money` ([Money](Description.md#moneybase))
2. `locale?` (string),
3. `options?` ([MoneyIntlOptions](Description.md#moneyintloptions))     
    

#### Returns

`string` 


**Example**

```js

import {createMoneyIntlFormatter} from "@easymoney/formatter"
import { createMoney } from '@easymoney/money';

const money = createMoney({amount: 5, currency: "USD"});
const money1 = createMoney({amount: 50, currency: "USD"});

const formatted = createMoneyIntlFormatter().format(money);
// => "$0.05"

const formatted1 = createMoneyIntlFormatter()
                    .format(money,
                            "en-US", 
                            {minimumFractionDigits: 1, maximumFractionDigits: 1});
// => "$0.5"

```