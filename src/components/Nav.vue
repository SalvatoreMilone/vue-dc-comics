<template>
  <div class="">
    <div class="nav">
        <ul>
          <li v-for="(element, index) in links" :key="index">
            <a :href="element.url" :class="{'active' : element.current}">{{element.text}}</a>
            <div class="selectednav" :class="{'active' : element.current}"></div>
          </li>
        </ul>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Nav',
  props: {
    msg: String
  },
  data() {
    return{
      links: [
        {
          text: "CHARACTERS",
          url:"#",
          current: false,
        },
        {
          text: "COMICS",
          url:"#",
          current: true,
        },
        {
          text: "MOVIES",
          url:"#",
          current: false,
        },
        {
          text: "TV",
          url:"#",
          current: false,
        },
        {
          text: "GAMES",
          url:"#",
          current: false,
        },
        {
          text: "COLLECTIBLES",
          url:"#",
          current: false,
        },
        {
          text: "VIDEOS",
          url:"#",
          current: false,
        },
        {
          text: "FANS",
          url:"#",
          current: false,
        },
        {
          text: "NEWS",
          url:"#",
          current: false,
        },
        {
          text: "SHOP",
          url:"#",
          current: false,
        },
      ]
    }
  }
}


</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
  ul{
    display: flex;
    flex-direction: row;
    align-items: center;
    list-style: none;
    

    li{
      margin: 0 5px;
      position: relative;
      height: var(--height1);
      display: flex;
      flex-direction: row;
      align-items: center;
      list-style: none;
    }
    a{
      text-decoration:none;
      color: black;
    }
  }
  .nav{
    height: var(--height1);
    display: flex;
    justify-content: flex-end;
    align-items: center;
  }
  .selectednav{
    height: 5px;
    width: 100%;
    background-color: var(--maincolor);
    position:absolute;
    bottom:0;
    display: none;
  }
  .active{
    color: #0282f9;
    display: block
  }
</style>
