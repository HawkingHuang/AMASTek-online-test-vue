<template>
  <v-container class="bg-brown-lighten-5 rounded-xl my-12 pa-8">
    <v-row align="center" justify="center">
      <v-col v-for="(variant, i) in variant1" :key="i" cols="auto">
        <v-card
          class="mx-auto bg-brown-lighten-3"
          max-width="344"
          :variant="variant"
        >
          <v-card-item>
            <div>
              <div class="mb-1 text-h6 text-md-h4 font-weight-bold">
                {{ variant[0] }}
              </div>
              <div class="text-body-1 text-md-h6 mb-1 text-center">
                {{ variant[1] }}
              </div>
            </div>
          </v-card-item>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
  <v-container class="bg-brown-lighten-5 rounded-xl my-10 pa-8">
    <v-row align="center" justify="center">
      <v-col v-for="(variant, i) in variant2" :key="i" cols="auto">
        <v-card
          class="mx-auto bg-brown-lighten-3"
          max-width="344"
          :variant="variant"
        >
          <v-card-item>
            <div>
              <div class="mb-1 text-h6 text-md-h4 font-weight-bold">
                {{ variant[0] }}
              </div>
              <div class="text-body-1 text-md-h6 mb-1 text-center">
                {{ variant[1] }}
              </div>
            </div>
          </v-card-item>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
  <v-container class="bg-brown-lighten-5 rounded-xl my-10 pa-8">
    <v-row align="center" justify="center">
      <v-col v-for="(variant, i) in variant3" :key="i" cols="auto">
        <v-card
          class="mx-auto bg-brown-lighten-3"
          max-width="344"
          :variant="variant"
        >
          <v-card-item>
            <div>
              <div class="mb-1 text-h6 text-md-h4 font-weight-bold">
                {{ variant[0] }}
              </div>
              <div class="text-body-1 text-md-h6 mb-1 text-center">
                {{ variant[1] }}
              </div>
            </div>
          </v-card-item>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>
<script setup>
const variant1 = [
  ["A", ""],
  ["冷凍庫溫度", "-10°C"],
  ["制冷", "1"],
  ["微壓差", "0.44 pa"],
  ["累積用電量", "1000 KWH"],
];
const variant2 = [
  ["B", ""],
  ["冷凍庫溫度", "-20°C"],
  ["制冷", "0"],
  ["微壓差", "0.02 pa"],
  ["累積用電量", "300 KWH"],
];
const variant3 = [
  ["C", ""],
  ["冷凍庫溫度", "-15°C"],
  ["制冷", "2"],
  ["微壓差", "0.28 pa"],
  ["累積用電量", "500 KWH"],
];
</script>

<script>
export default {};
</script>

<style></style>
