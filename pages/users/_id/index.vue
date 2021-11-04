<template>
  <div>
    <h4>it`s child #2</h4>
    <p>You clicked on</p>
    <h3>USER #{{ $route.params.id }}</h3>
    <v-btn color="primary" nuxt to="/users/_id/status"> status </v-btn>
  </div>
</template>

<script>
import Vue from "vue";
import Component from "nuxt-class-component";

export default
@Component({
  components: {},
})
class IdIndexPage extends Vue {}
</script>