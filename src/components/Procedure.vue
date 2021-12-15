<template>
  <section id="procedure" class="section-white">
    <div class="container">
      <div class="row">
        <div class="col text-center">
          <h6>HOW IT WORKS IN PRATICE</h6>
          <h2 class="my-4"><span><i class="far fa-gem"></i>Logitical</span> Procedure</h2>
          <p class="pb-3">We work with innovative methodologies to ensure that the entire delivery process is done from start to finish as planned.</p>
        </div>
      </div>
    </div>
    <div id="row-user" class="container-fluid"></div>
    <div id="service" class="container">
      <div class="row row-cols-5">
        <div class="col text-center">
          <div class="num">01</div>
          <h5 class="pb-2">Collection of information</h5>
          <p>Lorem ipsum dolor sit amet consectetur.</p>
        </div>
        <div class="col text-center">
          <div class="num">02</div>
          <h5 class="pb-2">Service Invoice Sending</h5>
          <p>Lorem ipsum dolor sit amet consectetur.</p>
        </div>
        <div class="col text-center">
          <div class="num">03</div>
          <h5 class="pb-2">Withdrawal of Cargo</h5>
          <p>Lorem ipsum dolor sit amet consectetur.</p>
        </div>
        <div class="col text-center">
          <div class="num">04</div>
          <h5 class="pb-2">Trasport Customer Order</h5>
          <p>Lorem ipsum dolor sit amet consectetur.</p>
        </div>
        <div class="col text-center">
          <div class="num">05</div>
          <h5 class="pb-2">Successful Delivery</h5>
          <p>Lorem ipsum dolor sit amet consectetur.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Procedure',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#row-user{
  border-top: 4px solid rgba($color: #52bbbb, $alpha: .25);
}
#service{
  .col{
    padding: 40px 12px;
    position: relative;

    .num{
      color: #52bbbb;
      font-weight: 900;
      background-color: rgba($color: #52bbbb, $alpha: .25);
      width: 40px;
      height: 40px;
      line-height: 40px;
      border-radius: 50%;
      position: absolute;
      left: 50%;
      top: -40px;
      transform: translate(-50%, 50%);
    }
  }
}

</style>
