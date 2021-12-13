<template>
  <nav id="navbar" class="container">
      <div id="logo">
        <a href="#"><span>NEX</span>GEN</a>
      </div>

      <div>
        <ul>
          <li><a href="#">HOME</a></li>
          <li><a href="#">ABOUT</a></li>
          <li><a href="#">SERVICES</a></li>
          <li><a href="#">PROCESS</a></li>
          <li><a href="#">TESTIMONIALS</a></li>
          <li><a href="#"><i class="far fa-user"></i></a></li>
          <button type="button" class="btn btn-user">GET IN TOUCH</button>
        </ul>
      </div>
  </nav>
</template>

<script>
export default {
  name: 'AppNavbar',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#navbar{
  font-size: 1.4rem;
  font-weight: bold;

  padding: .8rem 0;
  display: flex;
  justify-content: space-around;
  align-content: center;

  li{
    display: inline-block;
    cursor: pointer;
    padding: 0 1rem;
  }
  a{
    text-decoration: none;
    color: #c0c3d0;
  }
}
</style>
