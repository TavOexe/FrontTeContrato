<template>
  <v-flex>
    <v-card class=" overflow-hidden" height="1100">
        <navbar></navbar >
        <v-layout column align-center>
          <offers></offers>
          <offers></offers>
          <offers></offers>
        </v-layout>
    </v-card>
  </v-flex>
</template>

<script>
import navbar from "../components/navbar";
import offers from "../components/offers";
export default {
  name: "dashboard",
  components:{
    navbar,
    offers
  }
}
</script>

<style scoped>

</style>