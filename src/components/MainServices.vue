<template>
  <section id="mainservices" class="section-black">
      <div class="container">
          <div class="row">
              <div class="col">
                  <h6>ROAD TRANSPORT</h6>
                  <h2>Main <span>Services</span></h2>
              </div>
          </div>
          <div class="row">
              <div class="col-10">
                  <p>
                      With all of this expertise and capability comes an unrivalled commitment to customer service. We will work hard to understand your needs in order to develop a productive, long-term partnership.
                  </p>
              </div>
              <div class="col-2 text-end">
                  <button class="btn btn-user-secondary">SEE ALL</button>
              </div>
          </div>
          <div class="row row-cols-3">
                <Card v-for="item, i in servicesDetails"
                :key="i"
                :services="true" 
                :footer="false" 
                :descriptions="item"
            />
          </div>
      </div>
  </section>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
  name: 'MainServices',
  components: {
      Card
  },
  props: {
    servicesDetails: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.section-black{
    h6, h3{
        color: #52bbbb;
    }
    h2, h5{
        color: #fff;
        font-weight: 900;
    }

    h2{
        span{
            padding: .2rem 1rem;
            background-color: rgba($color: #52bbbb, $alpha: .4);
        }
    }

}


</style>
