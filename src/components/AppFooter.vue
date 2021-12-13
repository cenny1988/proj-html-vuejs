<template>
  <footer>
      <div class="container">
          <div class="row row-cols-4">
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
          </div>
      </div>
  </footer>
</template>

<script>
import Contact from '@/components/Contact.vue'

export default {
  name: 'AppFooter',
  components: {
      Contact
  },
  props: {
      contactsDetails: Array,
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
      padding: .4rem 0 .4rem 1.5rem;
      border-top-left-radius: 35px;
      border-bottom-left-radius: 35px;
      color: #52bbbb;
      background-color: rgba($color: #52bbbb, $alpha: .25);
    }

  }
}
</style>
