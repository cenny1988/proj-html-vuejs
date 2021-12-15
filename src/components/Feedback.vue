<template>
  <section id="feedback" class="section-black">
      <div id="results">
          <div class="container ">
              <div class="row text-center mb-3">
                  <div class="col">
                      <h6>WHAT ARE WE DOING</h6>
                      <h2><span>Results</span> in Numbers</h2>
                  </div>
              </div>
              <div class="row row-cols-2 row-cols-md-4 text-center">
                  <div class="col numbers">
                      <h3>128</h3>
                      <h5>Certifications</h5>
                  </div>
                  <div class="col numbers">
                      <h3>230</h3>
                      <h5>Employees</h5>
                  </div>
                  <div class="col numbers">
                      <h3>517</h3>
                      <h5>Customers</h5>
                  </div>
                  <div class="col numbers">
                      <h3>94</h3>
                      <h5>Countries Served</h5>
                  </div>
              </div>
          </div>
      </div>
        
      <div class="container py-5">
          <div class="row text-center mb-3">
              <div class="col">
                  <h6>CUSTOMER TESTIMONIALS</h6>
                  <h2>Trusted <span>Feedback</span></h2>
                  <p class="my-4">We work intensively in search of ideals than can add up in the lives of our customers. This is what moves us and we are grateful for the recognition.</p>
              </div>
          </div>
          <div class="row row-cols-1 row-cols-lg-3">
                <Card v-for="item, i in feed"
                :key="i" 
                :feedback="true" :footer="false" :descriptions="item"
                />
          </div>
      </div>

  </section>
</template>

<script>
import Card from '@/components/Card.vue'

export default {
  name: 'Feedback',
  components: {
      Card
  },
  props: {
    feed: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#feedback{
    padding-top: 0;
}
#results{
    min-height: 450px;
    background-image: url(../assets/img/bg-10.jpg);
    background-position: center;
    padding-top: 8rem;
    

    .numbers{
        padding-TOP: 3rem;
    }
}
</style>
