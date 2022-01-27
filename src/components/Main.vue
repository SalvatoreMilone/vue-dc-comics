<template>
  <div class="all">
    <div class="container">

    </div>
  </div>
</template>

<script>
export default {
  name: 'Main',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
  min-height: calc(100vh - var(--height1) - 600px);
  background-color: black;
}
</style>
