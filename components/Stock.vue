<template>
    <!-- text-center to center text -->
    <!-- Card to hold the stocks -->
    <v-container fluid>
        <v-card>
            <v-row>
                <v-col>
                    <v-card-title
                        dense
                        style="background-color: grey"
                    >
                        {{name}}
                    </v-card-title>
                </v-col>

                <v-col>
                    <v-card-text>
                        {{symbol}}
                    </v-card-text>
                </v-col>

            </v-row>
        </v-card>
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
