<template>
  <nav id="navbar" class="container">
    <div class="row">
      <div class="col-2 logo">
        <a href="#"><span>NEX</span>GEN</a>
      </div>
      
      <div class="col-2 text-end offset-8 d-lg-none" >
        <a href="#"><i class="fas fa-bars"></i></a>
      </div>

      <div class="col-10 d-none d-lg-block text-end">
        <ul>
          <li v-for="link,i in linksOptions" :key="i" :class="link.here ? 'active' : '' ">
            <a href="#">{{link.text}}</a>
          </li>
          <li><a href="#"><i class="far fa-user"></i></a></li>
          <button type="button" class="btn btn-user">GET IN TOUCH</button>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'AppNavbar',
  props: {
    linksOptions: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#navbar{
  font-size: 1rem;
  padding: .8rem 0;
  
  li{
    display: inline-block;
    cursor: pointer;
    padding: 0 1rem;

    &.active a, &:hover a{
      border-bottom: 1px solid #c0c3d0;
    }
  }
}
</style>
