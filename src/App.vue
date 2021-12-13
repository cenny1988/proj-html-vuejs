<template>
  <div id="app">
    <AppHeader :linksDetails="links"/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
  },
  data(){
      return{
          links: [
              {
                  text: "HOME",
                  url: "#",
                  here: false
              },
              {
                  text: "ABOUT",
                  url: "#",
                  here: true
              },
              {
                  text: "SERVICES",
                  url: "#",
                  here: false
              },
              {
                  text: "PROCESS",
                  url: "#",
                  here: false
              },
              {
                  text: "TESTIMONIALS",
                  url: "#",
                  here: false
              },
          ]
      }
  }
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  .btn{
    padding: 0.375rem 1.35rem;
  }
  .btn-user{
    color: #fff;
    background-color: #52bbbb;
    border-color: #52bbbb;
  }
  .btn-user-secondary{
    border: 1px solid #52bbbb;
    color: #fff;
  }
}
</style>
