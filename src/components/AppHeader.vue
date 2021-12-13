<template>
  <header>
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
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
  props: {
    
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
header{
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
            margin: 0 .7rem;
        }
        h6{
            display: inline-block;
        }
    }
}
</style>
