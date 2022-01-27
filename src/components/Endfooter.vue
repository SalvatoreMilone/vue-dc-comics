<template>
  <div class="">
    <div class="container">

      <div>
        <button>SIGN-UP NOW!</button>
      </div>

      <div>
        <span>FOLLOW US</span>
        <img src="../assets/img/footer-facebook.png">
        <img src="../assets/img/footer-periscope.png">
        <img src="../assets/img/footer-pinterest.png">
        <img src="../assets/img/footer-twitter.png">
        <img src="../assets/img/footer-youtube.png">
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'Topfooter',
  props: {
    msg: String
  },
  components: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
  height: 100px;
  background-color: #303030;
  display: flex;
  justify-content:space-between;
  align-items: center;
}

button{
  padding: 10px 15px;
  background-color: transparent;
  border: 3px solid var(--maincolor);
  color: white;
  font-size: 20px;
}

.container div:nth-child(2){
  color: var(--maincolor);
  display: flex;
  align-items: center;

  img{
    margin: 0 10px;
  }

  span{
    margin-right: 15px;
    font-size: 20px;
  }
}
</style>
