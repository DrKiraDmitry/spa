<template>
  <div>
    <navheader />
      <nuxt />
    <compfooter />
  </div>
</template>
<script>
import navheader from '~/components/navheader.vue'
import compfooter from '~/components/compfooter.vue'
export default {
  components:{
    navheader,
    compfooter
  }
}
</script>
<style>

</style>
