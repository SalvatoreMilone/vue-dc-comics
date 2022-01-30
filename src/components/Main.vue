<template>
  <div class="all">
        <div class="jumbotron">
          <button>CURRENT SERIES</button>
        </div>
    <div class="container">


        <Comicssection v-for="comic in Comics"
        :img="comic.thumb"
        :series="comic.series"
        :key="comic"/>

      <div class="btncontainer">
        <button>LOAD MORE</button>
      </div>

    </div>
  </div>
</template>

<script>
import Comicssection from './Comicssection.vue'
import Comics from "../../dc-comics.json";

export default {
  name: 'Main',
  props: {
  },
  components: {
    Comicssection,
  },
  data() {
    return{ 
      Comics
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
  min-height: calc(100vh - var(--height1) - 700px);
  background-color: #1c1c1c;
  padding-top: 20px;
  padding-bottom: 20px;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  flex-wrap: wrap;
  color: white;

  span{
      color: white;
      font-size: 28px;
  }
}

.jumbotron{
  height: 400px;
  width: 100%;
  background-image: url(../assets/img/jumbotron.jpg);
  background-size:cover;
  background-repeat: no-repeat;
  background-position: top;
  position: relative;

  button{
  position: absolute;
  bottom: -20px;
  left: 165px;
  }
}

button{
  padding: 10px 15px;
  background-color: var(--maincolor);
  color: white;
  border: none;
  font-size: 20px;
  cursor: pointer;
  transition: background-color 200ms;

  &:hover{
    background-color: rgb(0, 179, 255);
  }
}

.btncontainer{
  margin: 10px 0;
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
