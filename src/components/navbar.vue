<template>
  <v-flex>
  <v-app-bar color=#283593>
    <v-app-bar-nav-icon color="white" @click="drawer = true"></v-app-bar-nav-icon>
    <v-toolbar-title class="white--text" left>
      TeContrato
    </v-toolbar-title>
    <v-icon  x-large
             dark>mdi-account</v-icon>
    <v-icon  x-large
             dark>mdi-home</v-icon>
    <v-icon  x-large
             dark>mdi-notification</v-icon>
  </v-app-bar>
    <v-navigation-drawer
        v-model="drawer"
        absolute
        temporary
    >
      <v-list nav dense>
        <v-list-item-group v-model="group" active-class="black--text text--accent-4" color=#283593>
          <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-btn plain :to="{name: 'dashboard'} " >Home</v-btn>
          </v-list-item>
          <v-list-item >
            <v-list-item-icon>
              <v-icon>mdi-email</v-icon>
            </v-list-item-icon>
            <v-btn plain :to="{name: 'proyect'} " >Proyect</v-btn>
          </v-list-item>
          <v-list-item >
            <v-list-item-icon>
              <v-icon>mdi-message-text</v-icon>
            </v-list-item-icon>
            <v-btn plain :to="{name: 'configuration'} " >Configuration</v-btn>
          </v-list-item>
          <v-list-item >
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-btn plain :to="{name: 'Home'} " >Log out</v-btn>
          </v-list-item>
        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

  </v-flex>
</template>

<script>
import offers from "./offers";
export default {
  name: 'navbar',
  components:{
    offers,
  },
  data: () => ({
    drawer: false,
    group: null,
  }),
}
</script>
