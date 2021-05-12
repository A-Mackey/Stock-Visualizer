<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="4">
      <h1>test</h1>
      <v-col cols="4" v-for="{stock, index} in stocks" :key="index">
        <h1>test {{index}}</h1>
        <Stock name="stock.name" :symbol="stock.symbol" />
      </v-col>
    </v-col>
  </v-row>
</template>

<script>

import Stock from '../components/Stock'

export default {
  components: {
    Stock
  },

  data: {
    stocks: [
      { name: "Microsoft", symbol: "MSFT" },
      { name: "Apple", symbol: "AAPL" },
      { name: "Anheuser-Busch", symbol: "BUD" },
      { name: "S&P 500", symbol: "SPX" },
    ],
  },
}
</script>
