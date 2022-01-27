<template>
  <div class="">
    <div class="container">
      <div class="icons">
        <div><img src="../assets/img/buy-comics-digital-comics.png">DIGITAL COMICS</div>
        <div><img src="../assets/img/buy-comics-merchandise.png">DC MERCHANDISE</div>
        <div><img src="../assets/img/buy-comics-subscriptions.png">SUBSCRIPTION</div>
        <div><img src="../assets/img/buy-comics-shop-locator.png">COMIC SHOP LOCATOR</div>
        <div><img src="../assets/img/buy-dc-power-visa.svg">DC POWER VISA</div>
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
  height: var(--height1);
  background-color: var(--maincolor);
  color: white;
  font-size: 13px;
}
.icons{
  height: var(--height1);
  display: flex;
  justify-content: space-evenly;
  align-items: center;

  &>div{
    display: flex;
    justify-content: center;
    align-items: center;
  }
  &>div img{
    height: 60px;
    margin-right: 10px
  }
}

</style>
