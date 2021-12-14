<template>
  <main>
    <!-- who we are = contact form -->
    <WhoWeAre/>

    <!-- Main Services = trusted Feedback -->

    <!-- Logistical Procedure -->

    <!-- contact form -->
    <ContactForm :contactsArr="contactsDetails"/>

  </main>
</template>

<script>
import WhoWeAre from '@/components/WhoWeAre.vue'
import ContactForm from '@/components/ContactForm.vue'

export default {
  name: 'AppMain',
  components: {
    WhoWeAre,
    ContactForm
  },
  props: {
    contactsDetails: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>