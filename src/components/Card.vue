<template>
<section>
  <div class="col">
        <div class="card bg-dark-user">
            <div class="card-body">
              <!-- se non siamo nel footer head card.. -->
                <div v-if="!footer" class="icon mb-3">
                  <!-- se siamo nella sez services -->
                    <div v-if="services">
                      <span class="icon-service"><i :class="descriptions.icon"></i></span>
                      <span class="arrow"><i class="fas fa-arrow-right"></i></span>
                    </div>
                    <!-- se siamo nella sez feedback -->
                    <div v-if="feedback">
                      <img class="img-feed" :src="require(`../assets/img/${descriptions.img}`)">
                    </div>
                </div>
                <!-- se siamo nel footer corpo card-->
                <h4 v-if="footer" class="card-title text-white ">{{title}}</h4>
                <h4 v-else class="card-title text-white mb-3">{{descriptions.title}}</h4>
                <ul v-if="footer" class="fa-ul">
                    <li v-for="link, j in links" :key="j">
                        <a href="#"><span class="fa-li"><i class="fas fa-greater-than"></i></span>{{link.link}}</a>
                    </li>
                </ul>
                <!-- se NON siamo nel footer corpo card-->
                <p v-else>
                    {{descriptions.description}}
                    <span v-if="feedback" class="quotes"><i class="fas fa-quote-right fa-2x"></i></span>
                </p>
            </div>
        </div>
    </div>
</section>
</template>

<script>
export default {
  name: 'Card',
  props: {
    links: Array,
    title: String,
    footer: Boolean,
    descriptions: Array,
    services: Boolean,
    feedback: Boolean,
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card{
      background-color: #191c1e;
      min-height: 240px;

      .icon{
          margin: 0 1rem;
          color: #52bbbb;
          position: relative;

          img{
            height: 30%;
            filter: invert(1);
          }

          span.icon-service{
            display: inline-block;
        //   padding: 15px;
            text-align: center;
            line-height: 50px;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background-color: rgba($color: #52bbbb, $alpha: .25);
            font-size: 1.8rem;
          }

          span.arrow{
            color:  rgba($color: #52bbbb, $alpha: .25);
            font-size: 1.5rem;
            display: inline-block;
            position: absolute;
            top: 0;
            right: 0;
          }
      }

      span.quotes{
        color: rgba($color: #c0c3d0, $alpha: .25);
        position: absolute;
        right: 1rem;
        bottom: 1rem;
      }

      h4{
        margin-left: 1rem;
        font-weight: 700;
      }

      li{
        margin-bottom: .3rem;
      }

      p{
        margin: 0 1rem;
      }
}

</style>
