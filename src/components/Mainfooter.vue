<template>
  <div class="">
    <div class="container">
      <div class="subcontainer">

        <div>
          <span>DC COMICS</span>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
          </ul>
          <span>SHOP</span>
          <ul>
            <li>Shop DC</li>
            <li>Collectibles</li>
          </ul>
        </div>

        <div>
          <span>DC</span>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
          </ul>
        </div>

        <div>
          <span>SITES</span>
          <ul>
            <li>Characters</li>
            <li>Comics</li>
            <li>Movies</li>
            <li>TV</li>
            <li>Games</li>
          </ul>
        </div>


      </div>
        <img src="../assets/img/dc-logo-bg.png" >
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
  height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  align-items: center;
  color: white;
  overflow: hidden;
}
.subcontainer{
  display: flex;
  width: 100%;
}
span{
  font-size: 22px;
}

ul{
  margin-top: 15px;
  margin-bottom: 10px

}

.container > div ul{
  list-style:none;
}

.subcontainer > div{
  margin-right: 40px
}

.subcontainer > div li{
  opacity: .8;
  font-weight: 100px;
}

img{
  position: relative;
  right: 0px;
}

</style>
