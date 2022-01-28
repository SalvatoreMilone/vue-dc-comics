<template>
  <div class="">
    <div class="container">
      <div class="icons">
        <div v-for="(element, index) in links" :key="index">
          <img :src="element.url" :alt="element.text">
          {{element.text}}
        </div>
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
   data() {
    return{
      links: [
        {
          text: "DIGITAL COMICS",
          url: require('../assets/img/buy-comics-digital-comics.png'),
        },
        {
          text: "DC MERCHANDISE",
          url: require('../assets/img/buy-comics-merchandise.png'),
        },
        {
          text: "SUBSCRIPTION",
          url: require('../assets/img/buy-comics-subscriptions.png'),
        },
        {
          text: "COMIC SHOP LOCATOR",
          url: require('../assets/img/buy-comics-shop-locator.png'),
        },
        {
          text: "DC POWER VISA",
          url: require('../assets/img/buy-dc-power-visa.svg'),
        },
      ]
    }
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
