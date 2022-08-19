<template>
  <div class="home">
    <Luisa :design="figmaConfig" v-model="viewModel"/>
  </div>
</template>


<script>
import Vue from "vue";
import Luisa from "luisa-vue";
Vue.use(Luisa);

// import JSON file for deployment
import app from './app.json'

export default {
  name: "Home",
  data: function () {
    return {
      figmaJSON: app,
      figmaConfig: {
        figmaFile: "hV90BaZUwk4idT4ZY9FYLs",
        figmaAccessKey: "figd_8JkVWVqNHnkyEFqMv-NdxXH1KGVEKE8VlnR60hWX",
      },
      viewModel: {
        /**
         * Add your view model here
         */
      },
      config: {
        responsive: [
          { value: "Web", label: "Desktop", types: ["desktop"] },
          { value: "Mobile", label: "Mobile", types: ["tablet", "mobile"] },
        ],
        components: {
          /**
           * Register costum components here
           */
        },
      },
    };
  },
  components: {},
  methods: {
    /**
     * Place your methods here
     */
  },
};
</script>
