<template>
  <div class="">
    <div class="container">
      <Logo/>
      <Nav/>
    </div>
  </div>
</template>

<script>
import Logo from './Logo.vue'
import Nav from './Nav.vue'

export default {
  name: 'Header',
  props: {
    msg: String
  },
    components: {
      Logo,
      Nav
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
  height: var(--height1);
  background-color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>
