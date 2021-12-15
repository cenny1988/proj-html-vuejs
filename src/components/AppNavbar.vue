<template>
  <nav id="navbar" class="container">
      <div class="logo">
        <a href="#"><span>NEX</span>GEN</a>
      </div>

      <div>
        <ul>
          <li v-for="link,i in linksOptions" :key="i" :class="link.here ? 'active' : '' ">
            <a href="#">{{link.text}}</a>
          </li>
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
    linksOptions: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#navbar{
  font-size: 1.4rem;
  // .logo{
  //   font-weight: 600;
  //   letter-spacing: .5rem;

  //   span{
  //     padding: .6rem 0 .6rem 1.5rem;
  //     border-top-left-radius: 35px;
  //     border-bottom-left-radius: 35px;
  //     color: #52bbbb;
  //     background-color: rgba($color: #52bbbb, $alpha: .25);
  //   }
  // }

  padding: .8rem 0;
  display: flex;
  justify-content: space-around;
  align-content: center;

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
