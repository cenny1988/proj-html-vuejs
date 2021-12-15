<template>
  <section >
    <div  v-for="contact, i in contacts" :key="i" class="mb-2">
        <span :class="form? 'circle' : '' "><i :class="contact.icon"></i></span> 
        <div class="d-inline ps-2">{{contact.contact}}</div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Contact',
  props: {
    contacts: Array,
    form: Boolean,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
section{
  div{
    .circle{
        display: inline-block;
        text-align: center;
        line-height: 28px;
        border-radius: 50%;
        width: 28px;
        height: 28px;
        background-color: rgba($color: #52bbbb, $alpha: .4);
    }
    
    margin-right: 1rem;
    cursor: pointer;
    
  }
}
</style>
