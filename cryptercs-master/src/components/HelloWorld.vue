<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo.svg')"
          class="my-3"
          contain
          height="200"
        />
      </v-col>

      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Welcome to CryptoCS
        </h1>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts">
import Vue from "vue";
import services from "@/services";
export default Vue.extend({
  name: "HelloWorld",

  data: () => ({}),
  beforeMount() {
    services.crypter.example();
  }
});
</script>
