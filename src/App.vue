<template>
  <div id="app">
    <AppHeader :linksDetails="links" :contactsDetails="contacts"/>

    <AppMain :contactsDetails="contacts"/>

    <AppFooter 
      :contactsDetails="contacts"
      :aboutsLinks="abouts"
      :trasportLinks="trasports"
      :supportLinks="supports"
    />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppFooter from './components/AppFooter.vue'
import AppMain from './components/AppMain.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppFooter,
    AppMain,
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
          abouts:[
            {
              link: "The Company",
              url: "#"
            },
            {
              link: "Institutional",
              url: "#"
            },
            {
              link: "Social & Events",
              url: "#"
            },
            {
              link: "Innovation",
              url: "#"
            },
            {
              link: "Envoironment",
              url: "#"
            },
            {
              link: "Technology",
              url: "#"
            },
          ],
          trasports:[
            {
              link: "Industrialized",
              url: "#"
            },
            {
              link: "Chermicals",
              url: "#"
            },
            {
              link: "Packaged Liquids",
              url: "#"
            },
            {
              link: "Construction",
              url: "#"
            },
            {
              link: "Laminated Wood",
              url: "#"
            },
            {
              link: "And others",
              url: "#"
            },
          ],
          supports:[
            {
              link: "Responsibility",
              url: "#"
            },
            {
              link: "Terms of Use",
              url: "#"
            },
            {
              link: "About Cookies",
              url: "#"
            },
            {
              link: "Privacy Policy",
              url: "#"
            },
            {
              link: "Accessibility",
              url: "#"
            },
            {
              link: "Information",
              url: "#"
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
  $black-dark: #121117;
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
  .btn-user-info{
    border: 1px solid #52bbbb;
    color: #52bbbb;
  }
  a{
    text-decoration: none;
    color: #c0c3d0;
  }
  
}
</style>
