---
id: isZero
title: isZero
hide_title: true
sidebar_label: isZero
---


# `isZero()`

#### Returns

`boolean`


**Example**

```js

import { createMoney } from '@easymoney/money';

//if amount value is zero
const money = createMoney({ amount: 0, currency: 'USD' });

money.isZero();
// => true

//if amount value isnt zero
const money1 = createMoney({ amount: 100, currency: 'USD' });

money1.isZero();
// => false

```