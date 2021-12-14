<template>
    <div id="whoweare" class="section-white">
        <div class="container">
            <div class="row">
                <div class="col-9">
                    <h6>WHO WE ARE</h6>
                    <h2 class="my-4"><span><i class="far fa-gem"></i>Excellence</span> in Trasport</h2>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nostrum enim vitae animi, amet in mollitia veniam maxime perspiciatis sequi suscipit doloremque vero porro vel aut, iure eos illo impedit facere.</p>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nostrum enim vitae animi, amet in mollitia veniam maxime perspiciatis sequi suscipit doloremque vero porro vel aut, iure eos illo impedit facere.</p>
                    <div class="my-3 left-border">
                        <p> adipisicing elit. Sint nobis molestias vitae, suscipit laudantium voluptatibus optio sit, quia repellendus similique eius distinctio, maiores beatae quod rerum reprehenderit molestiae non! Eum?</p>
                    </div>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque laboriosam sunt error ipsam sit, molestiae autem quisquam</p>
                    <ul>
                        <li>lorem ipsumdolor sit amet</li>
                        <li>lorem ipsumdolor sit amet</li>
                        <li>lorem ipsumdolor sit amet</li>
                        <li>lorem ipsumdolor sit amet</li>
                        <li>lorem ipsumdolor sit amet</li>
                    </ul>
                </div>
                <div class="col-3">
                    <h5>Vehicle Type</h5>
                    <div class="my-1">
                        <div class="vehicle">
                            <div>
                                <img src="../assets/img/truck-1.png" alt="camion">
                            </div>
                            <div>
                                <h5>Light</h5>
                                Max Weight 1200 Kg
                            </div>
                        </div>
                        <div class="vehicle">
                            <div>
                                <img src="../assets/img/truck-1.png" alt="camion">
                            </div>
                            <div>
                                <h5>Light</h5>
                                Max Weight 1200 Kg
                            </div>
                        </div>
                        <div class="vehicle">
                            <div>
                                <img src="../assets/img/truck-1.png" alt="camion">
                            </div>
                            <div>
                                <h5>Light</h5>
                                Max Weight 1200 Kg
                            </div>
                        </div>
                    </div>
                    <h5>Certifications</h5>
                    <div class="half-width shadow">
                        <img src="../assets/img/certificate.png" alt="certified">
                    </div>
                    <div class="half-width invert-shadow">
                        <img src="../assets/img/certificate.png" alt="certified">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'WhoWeAre',
}
</script>

<style lang="scss">
// le stessw regole sono esportate anche per la sezione contact form
.section-white{
    background-color: #fff;
    padding: 5rem 0;

    h6, span{
        color: #52bbbb;
    }
    h2, h5{
        color: #000;
        font-weight: 900;
    }
    h2{
        font-weight: 900;

        span{
            padding: .2rem 1rem;
            background-color: rgba($color: #52bbbb, $alpha: .4);
        }

    }
    // style prte sinistra
    .left-border{
        border-left: rgba($color: #52bbbb, $alpha: .4) 5px solid;
        padding: .3rem 6rem .3rem 3rem;
    }


    // style parte destra
    .vehicle{
        display: flex;
        justify-content: flex-start;
        align-items: center;
        padding: .6rem 0;
        font-size: 1.2rem;

        div:first-child{
            width: 30%;
            margin-right: 1rem;
        
            img{
                background-color: #daeced;
                padding: .6rem;
                width: 100%;
            }
        }
        
        &:nth-child(2){
            border-top: 1px solid #daeced;
            border-bottom: 1px solid #daeced;
        }
    }

    .half-width{
        width: 50%;
        display: inline-block;
        padding: .5rem;
        

        img{
            width: 100%;
        }

    }
    .shadow{
        box-shadow: 10px 10px 10px 1px #daeced;
    }
    .invert-shadow{
        box-shadow: -10px 10px 10px 1px #daeced;
    }

}
</style>
