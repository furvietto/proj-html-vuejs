.<template>
<main>
    <div class="jumbotron container-fluid">
      <div class="row h-100">
          <div class="col-12 text-light back-jumbo position-relative">
              <!-- img jumbo -->
            <img class="h-100 w-50" src="./../assets/img/slide-1.jpg" alt="">
            <div class="row h-100">
                <div class="col-6 h-100">
                    <div class="row h-100 align-items-center justify-content-end">
                        <div class="col-9">
                            <h1 class="fw-bold mb-4">Udemy Affiliates Sales</h1>
                            <div class="fs-5">Monetize your audience and attract new customers with Udemy!</div>
                        </div>
                    </div>
                </div>
            </div>
          </div>
      </div>
  </div>
  <!-- popular courses -->
  <div class="pop-courses container">
      <div class="row">
          <div class="p-0 mb-3 col fs-5 fw-bold">
              Popular Development Courses
          </div>
      </div>
      <ul class="row row-cols-7 gap-3 list-unstyled">
          <li v-for="(card,index) in getArray" 
          :key="index"
          class="p-0 col card">           
              <img  :src="card.img" alt="">
              <div class="card-body">
                    <div class="development">
                        {{card.development}} <i class="fas fa-angle-right"></i>
                    </div>
                    <div class="description">
                        {{card.description}}
                    </div>
                    <div class="row align-items-center">
                        <div class="col-7">
                            <img v-for="(n,index) in 5" :key="index"
                            :src="(index < card.vote) ? require('./../assets/img/starfull.svg') : require('./../assets/img/staremptyl.svg')" alt="">
                            
                        </div>
                        <div class="col-5">
                            <div class="sale">
                                <del>
                                     {{card.sale}}
                                </del>                           
                            </div>
                            <div>
                                <strong>
                                      {{card.price}}
                                </strong>                          
                            </div>
                        </div>
                    </div>
              </div>
          </li>
      </ul>
  </div>
  <!-- popular courses -->

    <!-- learning -->
    <div class="container-fluid learning">
        <div class="row h-100 align-items-center">
            <div class="col-6">
                <div class="row justify-content-end">
                    <div class="col-8">
                        <h2 class="fw-bold">Limitless learning, more possibilities</h2>
                        <p class="mt-2 mb-4">Online courses open the oppurtinity for learning to almost anyone, regardless of their scheduling commitments</p>
                        <button type="button" class="read-more rounded-pill btn btn-danger">READ MORE</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- /learning -->

    <!-- recent courses -->
    <div class="container-fluid position-relative">
        <div class="row">
            <div class="col">
                <div class="container recent-courses">
                    <div class="row">
                        <div class="col ciao">
                            ciao
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- recent courses -->
</main>
  
</template>

<script>
export default {
    name:"Main",
    computed: {
         getArray:function () {
          return this.cards.filter((n,index) => {
                if (index < 6) {
                    return true
                }
            }); 
        }
    },

    data() {
        return {
            cards:[
                {
                    img:require("./../assets/img/895786_7b4b_2-272x161.jpg"),
                    development: "development",
                    description: "The Complete iOS 10 &amp; Swift 3 Developer Course",
                    sale: "$199.99",
                    price: "$100",
                    vote: 4,
                },
                {
                    img:require("./../assets/img/246154_d8b0_3-272x161.jpg"),
                    development: "development",
                    description: "Web Designer for beginners: Real Worls coding in HTML e CSS",
                    sale: "$129.99",
                    price: "$65",  
                    vote: 5,
                },
                {
                    img:require("./../assets/img/752950_b773-272x161.jpg"),
                    development: "development",
                    description: "GitHub Ultimate: Master Git and GitHub - Beginner to Expert",
                    sale: "$99.99",
                    price: "$50",
                    vote: 4,  
                },
                {
                    img:require("./../assets/img/1253188_58f7_2-272x161.jpg"),
                    development: "development",
                    description: "The Complete iOS 11 &amp; Swift Developer Course, Build 20 Apps",
                    sale: "$199.99",
                    price: "$100",
                    vote: 4  
                },
                {
                    img:require("./../assets/img/919872_ed54_6-272x161.jpg"),
                    development: "development",
                    description: "Android Java Masterclass - Become an App Developer",
                    sale: "$99.99",
                    price: "$100",
                    vote: 5, 
                },
                {
                    img:require("./../assets/img/951684_9c1a_2-272x161.jpg"),
                    development: "development",
                    description: "Xamarin Forms: Build Native Cross Platform Apps with C#",
                    sale: "$109.99",
                    price: "$95", 
                    vote: 5,
                },
            ]
        }
    },
    
}
</script>

<style lang="scss">
 @import "./../assets/scss/variables.scss";
.jumbotron{
    height: 40vh;
    margin: 20px 0;
    .back-jumbo{
        background-image: linear-gradient(65deg, $coral-red, $coral-red 55%, transparent 50%);
        img{
            position: absolute;
            top: 0;
            right: 0;
            z-index:-1;
        }
    }
}
.pop-courses{
    margin: 50px 0;
    height: 50vh;
        .development {
            font-size: 0.8em;
            margin-bottom: 10px;
            color: $venus;
        }
        .description {
            border-bottom: 1px solid black;
            padding-bottom: 15px;
        }
        .sale{
            font-size: 0.8em;
        }
}

.learning {
    background-image:url("./../assets/img/bg.png");
    height: 50vh;
    background-size: cover;
    background-position:center ;
    .read-more{
        font-size: 0.8em;
        padding: 13px 36px;
    }
    h2{
        font-size: 2.7em;
    }
}

.recent-courses {
    height: 80vh;
}
</style>