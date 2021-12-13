<template>
  <header >
      <!-- div con info orari e links social -->
    <div id="info-links">
        <div class="container">
            <div class="info">
                <div>
                    <i class="fas fa-clock"></i>
                    <h6>Open Hours : Mon - Sat - 9:00 - 18:00</h6>
                </div>
                <div>
                    <div>
                        <a href="#">
                            <i class="fas fa-phone-alt"></i>
                            <h6>+1 (305) 1234-5678</h6>
                        </a>
                    </div>
                    <div>
                        <a href="#">
                            <i class="fas fa-envelope"></i>
                            <h6>hello@example.com</h6>
                        </a>
                    </div>
                    <a href="#"><i class="fab fa-facebook"></i></a>
                    <a href="#"><i class="fab fa-twitter"></i></a>
                    <a href="#"><i class="fab fa-linkedin-in"></i></a>
                </div>
            </div>
        </div>
    </div>
    <!-- background con overlay -->
    <div class="bg-bgoverlay">
        <div class="overlay">
            <!-- navbar -->
            <AppNavbar :linksOptions="linksDetails"/>
            <!-- jumbo titolo e buttons -->
            <div class="container">
                <div id="jumbo-title" >
                    <h6>LOGISTICS SERVICES</h6>
                    <h1 class="h1 display-1">CARGO TRASPORT</h1>
                    <p>
                        Fractional or exclusive road cargo trasportation to all regins, with, small, medium and large vehicles
                    </p>
                    <button type="button" class="btn btn-user">GET IN TOUCH</button>
                    <button type="button" class="btn btn-user-secondary">READ MORE</button>
                </div>
            </div>
        </div>

    </div>

  </header>
</template>

<script>
import AppNavbar from '@/components/AppNavbar.vue'

export default {
  name: 'AppHeader',
  components: {
    AppNavbar,
  },
  props: {
      linksDetails: Array,
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
    color: #fff;
    .container{
        padding: 0;
        }

    // style della barra info grigia
    #info-links{
        background-color: #21333e;
        .info{
            padding: .7rem 0;
            color: #c0c3d0;

            display: flex;
            justify-content: space-between;


            a{
                text-decoration: none;
                color: #c0c3d0;
            }
            div:not(div:last-child){
                display: inline;
                margin-right: 2rem;
            }
            .svg-inline--fa{
                margin-right: .6rem;
            }
            h6{
                display: inline-block;
            }
        }
    }
    //style del background e del relativo overlay 
    .bg-bgoverlay{
    height: 700px;
    background-image: url(../assets/img/bg-9.jpg);
    background-position: top;
    background-size: cover;

    position: relative;

    .overlay{
        height: 100%;
        background-color: rgba($color: #000000, $alpha: .5);
        }

        #jumbo-title{
            padding: 100px 0;
            width: 40%;

            h6{
                color: #52bbbb;
            }

            h1{
                font-weight: bold;
            }

            p{
                color: #c0c3d0;
                font-size: 1.2rem;
                margin-bottom: 1.5rem;
            }

            button{
                margin-right: 1rem;
            }
        }
    }
}
</style>
