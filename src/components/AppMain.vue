<template>
  <main>
    <!-- who we are = contact form -->
    <WhoWeAre/>

    <!-- Main Services = trusted Feedback -->
    <MainServices :servicesDetails="services"/>

    <!-- Logistical Procedure -->
    <Procedure/>

    <!-- trusted Feedback -->
    <Feedback :feed="feedbacks"/>
    
    <!-- contact form -->
    <ContactForm :contactsArr="contactsDetails"/>

  </main>
</template>

<script>
import WhoWeAre from '@/components/WhoWeAre.vue'
import ContactForm from '@/components/ContactForm.vue'
import MainServices from '@/components/MainServices.vue'
import Feedback from '@/components/Feedback.vue'
import Procedure from '@/components/Procedure.vue'

export default {
  name: 'AppMain',
  components: {
    WhoWeAre,
    ContactForm,
    MainServices,
    Feedback,
    Procedure
  },
  props: {
    contactsDetails: Array,
  },
  data() {
      return {
          services: [
              {
                  icon: "fas fa-microchip",
                  title: "Technology",
                  description: "We are continually focused on developing technology solutions adapted to our client's needs."
              },
              {
                  icon: "fas fa-temperature-low",
                  title: "Reefer Cargo",
                  description: "Regular and frequent monitoring from the receipt of the loaded conteiner to final destination."
              },
              {
                  icon: "fas fa-truck",
                  title: "Dry Cargo",
                  description: "We work with most types of dry cargo, from valuable cargo to the most dangerous requiring care."
              },

          ],
          feedbacks: [
              {
                  img: "logo-1.png",
                  description: "Lorem ipsum dolor sit, amet consectetur adipisicing elit. Delectus blanditiis enim cumque fuga. Voluptatum minus libero distinctio facilis rem mollitia sapiente minima. Perferendis quia saepe nobis enim cumque, ab architecto."
              },
              {
                  img: "logo-2.png",
                  description: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis quas reprehenderit eaque, vel cupiditate recusandae odio ducimus dolorem inventore, deleniti nulla? Earum dicta quibusdam, eum pariatur possimus repudiandae vel dolor?"
              },
              {
                  img: "logo-3.png",
                  description: "Lorem ipsum dolor sit amet consectetur, adipisicing elit. Corporis quas reprehenderit eaque, vel cupiditate recusandae odio ducimus dolorem inventore, deleniti nulla? Earum dicta quibusdam, eum pariatur possimus repudiandae vel dolor?"
              },

          ],
      }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>