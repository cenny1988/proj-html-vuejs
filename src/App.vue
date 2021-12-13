<template>
  <div id="app">
    <AppHeader :linksDetails="links" :contactsDetails="contacts"/>

    <AppFooter :contactsDetails="contacts"/>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
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
          ],
          contacts: [
            {
              icon: "fas fa-phone-alt",
              contact: "+1(305)1234-5678"
            },
            {
              icon: "fas fa-envelope",
              contact: "hello@example.com"
            },
            {
              icon: "fas fa-map-marker-alt",
              contact: "Main Avenue, 987"
            },
          ],
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
  color: #c0c3d0;

  .btn{
    padding: 0.375rem 1.35rem;
    font-weight: 500;
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
  a{
    text-decoration: none;
    color: #c0c3d0;
  }
  
}
</style>
