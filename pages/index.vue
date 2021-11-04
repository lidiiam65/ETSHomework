<template>
  <div>
    <div class="menu">
      <h1>Home page</h1>
      <v-row>
        <v-col>
          <v-btn color="primary" nuxt to="/users"> Users </v-btn>
          <v-btn color="primary" nuxt to="/about"> About </v-btn>
          <v-btn color="primary" nuxt to="/inspire"> Inspiration </v-btn>
        </v-col>
      </v-row>
    </div>
  </div>
</template>

<style>
.menu{
  width: 100%;
  cursor: pointer;
}
</style>

<script>
import Vue from "vue";
import Component from "nuxt-class-component";

export default
@Component({
  components: {},
})
class Index extends Vue {}
</script>
