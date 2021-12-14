<template>
  <div class="col">
        <div class="card bg-dark-user" v-for=" link, i in links" :key="i">
            <div class="card-body">
                <h5 class="card-title text-white">{{link.key}}</h5>
                <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Vitae et quidem quaerat, quae deserunt modi natus</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    links: Object
  },
  methods: {
      print(item){
          console.log(item);
          
      }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.card{
      background-color: #191c1e;
}

</style>
