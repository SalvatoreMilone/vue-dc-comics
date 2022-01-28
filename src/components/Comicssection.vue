<template>
  <div class="all">
    <div class="comic-container">
      <div class="comic">
        <img :src="img" alt="test">
      </div>
      <div>{{series}}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Comicssection',
  props: {
    img: String,
    series: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.comic{
  height: 200px;
  width: 200px;
  overflow: hidden;
  margin-bottom: 5px;

  img{
    width: 100%;
  }
}

.comic-container{
  width: 200px;
    margin: 14px 5px;
}
</style>
