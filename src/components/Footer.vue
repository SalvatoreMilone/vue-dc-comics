<template>
  <div class="">
    <Topfooter/> 
    <Mainfooter/> 
    <Endfooter/> 
  </div>
</template>

<script>
import Topfooter from './Topfooter.vue'
import Mainfooter from './Mainfooter.vue'
import Endfooter from './Endfooter.vue'

export default {
  name: 'Footer',
  props: {
    msg: String
  },
  components: {
    Topfooter,
    Mainfooter,
    Endfooter
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
  height: 600px;
}
</style>
