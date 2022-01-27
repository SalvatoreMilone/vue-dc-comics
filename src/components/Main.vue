<template>
  <div class="all">
    <div class="container">
         <span> --> Content goes here</span>
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
  padding-top: 10px;
  padding-bottom: 10px;
  display: flex;
  justify-content: flex-start;
  align-items: center;

  span{
      color: white;
      font-size: 28px;
  }
}
</style>
