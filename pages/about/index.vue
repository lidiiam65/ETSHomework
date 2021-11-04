<template>
  <div>
    <h4>It`s child`s info</h4>
    <p></p>

    <p @click="goToParagraph(1)" class="btnClck">
      Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam rhoncus
      euismod facilisis.
    </p>
    <p @click="goToParagraph(2)" class="btnClck">
      Pellentesque aliquam a purus quis suscipit. Vestibulum metus metus,
      dignissim id quam nec, pellentesque ornare est. Morbi porttitor
      sollicitudin turpis, nec sollicitudin tortor lobortis non.
    </p>
    <p @click="goToParagraph(3)" class="btnClck">
      Etiam elit quam, viverra non tellus a, venenatis cursus magna. Interdum et
      malesuada fames ac ante ipsum primis in faucibus. Nam auctor in diam quis
      hendrerit. Orci varius natoque penatibus et magnis dis parturient montes,
      nascetur ridiculus mus.
    </p>
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
class About extends Vue {
  goToParagraph(id) {
    this.$router.push({ path: `/about/${id}` });
  }
}
</script>
