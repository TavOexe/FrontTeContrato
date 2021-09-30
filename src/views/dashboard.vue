<template>
  <v-flex>
      <v-card column>
        <navbar></navbar >

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
    offers,
  }
}
</script>

<style scoped>

</style>