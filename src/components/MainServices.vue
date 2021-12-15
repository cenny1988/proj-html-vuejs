<template>
  <section id="mainservices" class="section-black">
      <div class="container">
          <div class="row">
              <div class="col">
                  <h6>ROAD TRANSPORT</h6>
                  <h2>Main Services</h2>
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
          <div class="row">
              <div class="col-4">
                  <Card :footer="false" :descriptions="servicesDetails[0]"/>
              </div>
              <div class="col-4">
                  <Card :footer="false" :descriptions="servicesDetails[1]"/>
              </div>
              <div class="col-4">
                  <Card :footer="false" :descriptions="servicesDetails[2]"/>
              </div>
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
    h6{
        color: #52bbbb;
    }
    h2, h5{
        color: #fff;
        font-weight: 900;
    }

}


</style>
