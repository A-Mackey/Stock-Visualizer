<template>
  <v-container fluid>

      <v-row>
            <v-col 
              xs="12"
              sm="12" 
              md="6" 
              lg="4" 
              xl="3"
              v-for="stock, i in stocks" 
              :key="i"
            >

                <StockModule 
                  :name="stock.name"
                  :symbol="stock.symbol"
                />
            </v-col>
        </v-row>
  </v-container>
</template>

<script>

import StockModule from '../components/Stock'

export default {
  components: {
    StockModule
  },

  data () {
    return {
      stocks: [
        { name: "Microsoft", symbol: "MSFT" },
        { name: "Apple", symbol: "AAPL" },
        { name: "Anheuser-Busch", symbol: "BUD" },
        { name: "S&P 500", symbol: "SPX" },
      ],
      options: { }
    }
  }
}
</script>
