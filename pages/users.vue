<template>
  <div>
    <h1>USERS</h1>
    <h2>it`s parent</h2>
    <p></p>
    <nuxt-child />
    <p></p>
    <v-btn color="primary" nuxt to="/"> Homepage </v-btn>
  </div>
</template>

<style>
</style>

<script>
import Vue from "vue";
import Component from "nuxt-class-component";

export default
@Component({
  components: {},
})
class Users extends Vue {}
</script>