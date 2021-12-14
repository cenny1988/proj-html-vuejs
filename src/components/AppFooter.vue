<template>
<div>
  <footer>
      <div class="container">
          <div class="row row-cols-4">
              <!-- col1 -->
              <div class="col">
                <div class="logo mb-3">
                    <a href="#"><span>NEX</span>GEN</a>
                </div>
                <div class="mb-3">
                    A Functional HTML Template for Corporate & Business
                </div>
                <Contact :contacts="contactsDetails"/>
                <button type="button" class="btn btn-user-secondary mt-3">GET IT Touch</button>
              </div>

              <!-- col2 -->
              <Card :title="'About'" :links="aboutsLinks"/>

              <!-- col3 -->
              <Card :title="'Trasport'" :links="trasportLinks"/>

              <!-- col4 -->
              <Card :title="'Support'" :links="supportLinks"/>
          </div>
      </div>

  </footer>
  <div id="copyright">
    <div class="container">
      <div class="row row-cols-2">
        <div class="col">
          Enjoy the low price. We are tracking any intention of piracy.
        </div>
        <div class="col text-end">
          &#169; 2020 NEXGEN is Proudly Powered by <span>Codings</span>.
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
import Contact from '@/components/Contact.vue'
import Card from '@/components/Card.vue'

export default {
  name: 'AppFooter',
  components: {
      Contact,
      Card
  },
  props: {
      contactsDetails: Array,
      aboutsLinks: Array,
      trasportLinks: Array,
      supportLinks: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer{
    background-color: #121117;
    padding: 4rem 0;

    .logo{
    font-weight: 600;
    letter-spacing: .5rem;

    span{
      padding: .6rem 0 .6rem 1.5rem;
      border-top-left-radius: 35px;
      border-bottom-left-radius: 35px;
      color: #52bbbb;
      background-color: rgba($color: #52bbbb, $alpha: .25);
      }

    }

}
#copyright{
  background-color: #0d0d11;
  padding: 1rem 0;
  font-size: .8rem;

  span{
    color: #52bbbb;
  }
}
</style>
