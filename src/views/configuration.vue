<template>
  <v-flex>
    <v-card class=" overflow-hidden" height="1100">
      <navbar></navbar >
      <v-layout column align-center>

      </v-layout>
    </v-card>
  </v-flex>
</template>

<script>
import navbar from "../components/navbar";
export default {
  name: "configuration",
  components:{
    navbar,
  }
}
</script>

<style scoped>

</style>