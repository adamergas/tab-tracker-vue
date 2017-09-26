<template>
  <v-toolbar fixed class="cyan" dark>
    <v-toolbar-title class="mr-4">
      <router-link to="home" tag="span" class="home">Tab Tracker</router-link>
    </v-toolbar-title>
    <!--Do Later-->
    <!--<v-toolbar-items>
      <v-btn flat dark>
        Browse
      </v-btn>
    </v-toolbar-items>-->
    <v-spacer></v-spacer>
    <v-toolbar-items>
      <v-btn flat dark to="login" v-if="!$store.state.isUserLoggedIn">
        Log In
      </v-btn>
      <v-btn flat dark to="register" v-if="!$store.state.isUserLoggedIn">
        Sign Up
      </v-btn>
    </v-toolbar-items>
  </v-toolbar>
</template>

<script>
export default {

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.home {
  cursor: pointer;
}
.home:hover {
  color:#EEE;
}
</style>
