<template>
  <div class="">
    <div class="container">

    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
  height: var(--height1);
  background-color: white;
}
</style>
