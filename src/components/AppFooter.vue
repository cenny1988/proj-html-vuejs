<template>
<div>
  <footer class="section-black">
      <div class="container">
          <div class="row row-cols-1 row-cols-sm-2 row-cols-lg-4 ">
              <!-- col1 -->
              <div class="col">
                <div class="logo mb-3">
                    <a href="#"><span>NEX</span>GEN</a>
                </div>
                <div class="mb-3">
                    A Functional HTML Template for Corporate & Business
                </div>
                <Contact :form="false" :contacts="contactsDetails"/>
                <button type="button" class="btn btn-user-secondary mt-3">GET IT Touch</button>
              </div>

              <!-- col2 -->
              <Card :footer="true" :title="'About'" :links="aboutsLinks"/>

              <!-- col3 -->
              <Card :footer="true" :title="'Trasport'" :links="trasportLinks"/>

              <!-- col4 -->
              <Card :footer="true" :title="'Support'" :links="supportLinks"/>
          </div>
      </div>

  </footer>
  <div id="copyright">
    <div class="container">
      <div class="row row-cols-1 row-cols-md-2">
        <div class="col">
          Enjoy the low price. We are tracking any intention of piracy.
        </div>
        <div class="col text-md-end">
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


#copyright{
  background-color: #0d0d11;
  padding: 1rem 0;
  font-size: .8rem;

  span{
    color: #52bbbb;
  }
}
</style>
