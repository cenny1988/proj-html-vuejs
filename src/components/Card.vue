<template>
<section>
  <div class="col">
        <div class="card bg-dark-user">
            <div class="card-body">
                <h4 class="card-title text-white">{{title}}</h4>
                <ul class="fa-ul">
                    <li v-for="link, j in links" :key="j">
                        <a href="#"><span class="fa-li"><i class="fas fa-greater-than"></i></span>{{link.link}}</a>
                    </li>
                </ul>
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
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card{
      background-color: #191c1e;

      h4{
          margin-left: 1rem;
          font-weight: 700;
      }

      li{
          margin-bottom: .3rem;
      }
}

</style>
