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
  $black-user: #121117;
  $green-user: #52bbbb;
  $gray-user: #c0c3d0;
  $white-user: #fff;

  color: $gray-user;

  .btn{
    padding: 0.375rem 1.35rem;
    font-weight: 500;
  }
  .btn-user{
    color: $white-user;
    background-color: $green-user;
    border-color: $green-user;
  }
  .btn-user-secondary{
    border: 1px solid $green-user;
    color: $white-user;
  }
  .btn-user-info{
    border: 1px solid $green-user;
    color: $green-user;
  }
  a{
    text-decoration: none;
    color: $gray-user;
  }
// stile logo
  .logo{
    font-weight: 600;
    letter-spacing: .5rem;

    span{
      padding: .6rem 0 .6rem 1.5rem;
      border-top-left-radius: 35px;
      border-bottom-left-radius: 35px;
      color: $green-user;
      background-color: rgba($green-user, $alpha: .25);
    }
  }
// stile sezioni black
  .section-black{
    background-color: $black-user;
    padding: 5rem 0;
  }
}
// stile sezioni white
.section-white{
    background-color: #fff;
    padding: 5rem 0;

    h6, span{
        color: #52bbbb;
    }
    h2, h5{
        color: #000;
        font-weight: 900;
    }
    h2{
        font-weight: 900;

        span{
            padding: .2rem 1rem;
            background-color: rgba($color: #52bbbb, $alpha: .4);
        }

    }
}
</style>
