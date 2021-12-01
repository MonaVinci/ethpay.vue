# ETHPay for Vue.js

A Button to the Web3, [Demo](https://ethpay.now.sh/demo1)

## Quick Start

For Vue.js developers, just install it from NPM:

```bash
npm i ethpay.vue
```

## Vue.js Usage

```vue
<template>
  <div id="app">
    <ETHPay
      caption="Try with"
      to="0x8c7aF1e533Db27dB801F080898F0b81620208594"
      title="Pay ETH With MetaMask"
      value="0.1"
    />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import ETHPay from "ethpay.vue";
import "ethpay.vue/dist/ethpay.vue.css";

@Component({
  components: {
    ETHPay
  }
})
export default class App extends Vue {}
</script>
```

| Props | Desc | Type | Required |
|---|---|---|---|
| currency | Currency symbol | 'eth' | Yes |
| to | Address | String | Yes |
| value | The amount of currency | Number | Yes |
| caption | Button caption | String | No |
| title | HTML Title | String | No |
| data | The data append to Tx | String, starts with '0x' | No |

## Typescript

Typescript is supported.

## LISENCE

MPL-2.0
