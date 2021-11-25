<template>
  <div class="hello">
      <Comic/>
  </div>
</template>

<script>
import Comic from '../components/Comic.vue';

export default {
  name: 'Comics',
  components: {
      Comic,
  },

  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>