<template>
  <section >
    <div  v-for="contact, i in contacts" :key="i" class="mb-2">
        <span class="circle"><i :class="contact.icon"></i></span> {{contact.contact}}
    </div>
  </section>
</template>

<script>
export default {
  name: 'Contact',
  props: {
    contacts: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section{
  div{
    
    margin-right: 1rem;
    cursor: pointer;
    
    .svg-inline--fa{
      margin-right: .4rem;
    }
  }
}
</style>
