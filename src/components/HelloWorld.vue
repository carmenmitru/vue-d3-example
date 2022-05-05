<template>
  <v-app>
    <v-container>
      <v-row>
        <v-col cols="4" class="d-flex justify-center align-center">
          <h3 class="pb-2">Countries in 2021 with the highest GDP</h3>
          <div class="pa-2">
            <BarChart
              class="chart"
              :data-set="data"
              :margin-left="40"
              :margin-top="40"
              :tick-count="5"
              :bar-padding="0.5"
            />
          </div>
        </v-col>
        <v-col id="arc" />
      </v-row>
    </v-container>
  </v-app>
</template>

<script>
import BarChart from "@/components/BarChart.vue";

export default {
  name: "HelloWorld",
  data() {
    return {
      data: [
        ["USA", 20.5],
         ["China", 30],
        ["UK", 13.4],
        ["Spain", 22],
        ["Germany", 19],
        ["France", 38],
        ["Hungary", 21],
        ["Kirsty", 25],
       
        ["Ukraine", 17],
      ],

    };
  },
  components: {
    BarChart,
    
  },
};
</script>


