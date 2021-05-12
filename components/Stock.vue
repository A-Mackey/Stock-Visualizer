<template>
    <v-container>
        <h1>{{name}} : {{symbol}}</h1>
    </v-container>
</template>

<script>

export default {
  components: {
  },

  props: {
      name: String,
      symbol: String,
  }
}
</script>
