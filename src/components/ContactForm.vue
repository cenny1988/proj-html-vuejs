<template>
    <div id="contactform" class="section-white">
        <div class="container">
            <div class="row">
                <div class="col-9">
                    <h6>SEND A MESSAGE</h6>
                    <h2 class="my-4">Get in <span>Touch</span></h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                    <!-- form group -->
                    <div id="form-input" class="row g-3">
                        <!-- Name and email -->
                        <div class="col-6">
                            <input type="text" class="form-control" placeholder="Name">
                        </div>
                        <div class="col-6">
                            <input type="email" class="form-control" placeholder="Email">
                        </div>
                        <!-- phone and inf -->
                        <div class="col-6">
                            <input type="number" class="form-control" placeholder="Phone">
                        </div>
                        <div class="col-6">
                            <select class="form-select">
                                <option selected>More Info</option>
                                <option>...</option>
                            </select>
                        </div>
                        <!-- message -->
                        <div class="col">
                            <textarea class="form-control" id="exampleFormControlTextarea1" rows="5" placeholder="Message"></textarea>
                        </div>
                    </div>
                    <button class="btn btn-user my-4">SEND</button>
                </div>
                <div class="col-3">
                    <h5>Example Inc.</h5>
                    <p> nisi sed doloremque recusandae quos laudantium incidunt!</p>
                    <p> nisi sed doloremque recusandae quos laudantium incidunt!</p>
                    <Contact class="green-circle my-4" :contacts="contactsArr"/>

                    <button class="btn btn-user-info">VIEW MAP</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Contact from '@/components/Contact.vue'

export default {
  name: 'ContactForm',
  components: {
    Contact,
  },
  props: {
    contactsArr: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
#form-input{
    .form-control, .form-select{
        background-color: #ececec;
        color: #c0c3d0;
    }
}

.green-circle{
    span .circle{
        display: inline-block;
        width: 1rem;
        height: 1rem;
        background-color: rgba($color: #52bbbb, $alpha: .4);
        // color: #52bbbb;

        .svg-inline--fa{
            font-size: 2rem;
        }

    }
}
</style>
