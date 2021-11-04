<template>
  <div>
    <p>it was paragraph #{{ $route.params.id }}</p>
  </div>
</template>

<script>
import Vue from "vue";
import Component from "nuxt-class-component";

export default
@Component({
  components: {},
})
class IdPage extends Vue {}
</script>