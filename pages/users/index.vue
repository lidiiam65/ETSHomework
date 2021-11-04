<template>
  <div>
    <h4>it`s child #1</h4>
    <ul>
      <li @click="goToUser(1)" class="btnClck">User #1</li>
      <li @click="goToUser(2)" class="btnClck">User #2</li>
      <li @click="goToUser(3)" class="btnClck">User #3</li>
      <li @click="goToUser(4)" class="btnClck">User #4</li>
    </ul>
  </div>
</template>

<style>
.btnClck {
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
class Users extends Vue {
  goToUser(id) {
    this.$router.push({ path: `/users/${id}` });
  }
}
</script>