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
          <div class=" mb-3 col fs-5 fw-bold">
              Popular Development Courses
          </div>
      </div>
      <ul class="row row-cols-6 list-unstyled">
          <Card 
          v-for="(card,index) in getArray" 
          :key="index"
          :card="card"
          />
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
                        <button type="button" class="read-more rounded-pill btn-outline-danger">READ MORE</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- /learning -->

    <!-- recent courses -->
    <div class="container-fluid mt-5 mb-5 position-relative">
        <div class="row">
            <div class="col">
                <div class="container recent-courses">
                    <div class="row">
                        <div class="col text-center">
                            <h3 class="fw-bold fs-2">Recent Courses</h3>
                        </div>
                    </div>
                    <div class="row justify-content-center">
                        <div class="col-9">
                            <ul class="mb-5 mt-4 align-items-center recent-courses-list list-unstyled text-center row justify-content-between">
                                <li class="col-2 clicked">
                                    All Categories
                                </li>
                                <li class="col">                               
                                        Business
                                </li>
                                <li class="col">                                  
                                        Design
                                </li>
                                <li class="col">
                                    Development
                                </li>
                                <li class="col-2">
                                    IT &amp; software
                                </li>
                                <li class="col">
                                    Lifestyle
                                </li>
                                <li class="col">
                                    Marketing
                                </li>
                                <li class="col-2">
                                    Office Productivity
                                </li>
                            </ul>
                        </div>
                    </div>
                    <ul class="list-unstyled mb-5 row row-cols-6">
                        <Card 
                        v-for="(card,index) in cards" 
                        :key="index"
                        :card="card"
                        />
                    </ul>
                    <div class="row">
                        <div class="col-12 text-center">
                            <button type="button" class="show-all rounded-pill btn btn-outline-danger">SHOW ALL</button>
                        </div>
                    </div>
                    <div class="rigth-menu flex-column row">
                        <div class="col p-2">
                            <i class="fas fa-desktop"></i>
                        </div>
                        <div class="col p-2">
                            <i class="far fa-life-ring"></i>
                        </div>
                        <div class="col p-2">
                            <i class="fas fa-wrench"></i>
                        </div>
                        <div class="col p-2">
                            <i class="fas fa-shopping-cart"></i>
                        </div>
                        <div class="col d-flex justify-content-center p-2">
                            <i class="fas fa-mobile-alt"></i>
                        </div>
                    </div>
                </div>
            </div>   
        </div>
    </div>
    <!-- recent courses -->

    <!-- subscribe -->
    <div class="subscribe container-fluid">
        <div class="row h-100 align-items-center justify-content-center">
            <div class="col-8">
                <div class="row text-white">
                    <div class="col">
                        <h4>Suscribe our newsletter</h4>
                        <p>There are variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words</p>
                    </div>
                    <div class="col">
                        <div class="mb-3">
                            YOUR EMAIL ADDRESS
                        </div>
                        <input class="w-75 p-2" placeholder="Enter your E-mail" type="text">
                        <button class="p-2">SUBSCRIBE</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- subscribe -->

    <!-- popular courses -->
    <div class="container-fluid popular-courses ">
        <div class="row">
            <div class="col">
                <div class="container mt-5">
                    <div class="row">
                        <div class="col text-center">
                            <h3 class="fw-bold fs-2">Recent Courses</h3>
                        </div>
                    </div>
                    <div class="row">
                        <div class="col text-center">
                            <div>Discover our most popular courses for self learning</div>
                        </div>
                    </div>
                    <ul class="list-unstyled mt-5 mb-5 row row-cols-6">
                        <Card 
                        v-for="(card,index) in getArray" 
                        :key="index"
                        :card="card"
                        />
                    </ul>
                    <div class="row mb-5">
                        <div class="col text-center">
                            <button>
                                <i class="fas fa-angle-left"></i>
                            </button>
                            <button >
                                <i class="fas fa-angle-right"></i>
                            </button>                          
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- /popular courses -->

    <!-- work with us -->
    <div class="work-with-us mt-5 mb-5 container">
        <div class="row gap-3">
            <div class="col border">
                <div class="p-5 row align-items-center">
                    <div class="col-5">
                        <img src="./../assets/img/image_box_1-221x231.png" alt="">
                    </div>
                    <div class="col-7">
                        <h3>Become an instructor</h3>
                        <p>Teach what you love. Masterstudy gives you the tools to create a course</p>
                        <button type="button" class="shadow-none rounded-pill btn btn-danger">START TEACHING</button>
                    </div>
                </div>
            </div>
            <div class="col border">
                <div class="p-5 row align-items-center">
                    <div class="col-5">
                        <img src="./../assets/img/image_box_2-234x231.png" alt="">
                    </div>
                    <div class="col-7">
                        <h3>Access For Business</h3>
                        <p>Get unlimited access to 2,500 of top courses for your team</p>
                        <button type="button" class="shadow-none rounded-pill btn btn-danger">DOING BUSINESS</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!--/work with us -->

    <!-- investing -->
    <div class="investing pb-5 pt-5 container-fluid">
        <div class="row h-100">
            <div class="col">
                <div class="container pt-4 pb-4 h-100">
                    <div class="row h-100">
                        <div class="col-8">
                            <div class="row h-100 justify-content-end">
                                <div class="col-10">
                                    <div class="row align-items-center h-100">
                                        <div class="cartoon h-100 col-11">
                                            <h3>Investing for Your Future</h3>
                                            <p class=" mt-4 mb-4">It is no exaggeration to say this Masterstudy experience was trasformative-both professionally and personally. This workshop will long remain a high point of my life. Thanks again... I am feeling energized and eager to start teaching my class next week. I can't wait to use all of my new teaching tools. I will absolutely recommend this workshop to other educators!</p>
                                            <div class="fw-bold">Linda Green</div>
                                            <div class="sign">Product Manager, Apple Inc</div>
                                        </div>
                                        <div class="triangle col-1">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- /investing -->
</main>
  
</template>

<script>
import Card from './Card.vue'

export default {
    components:{
        Card
    },
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
                {
                    img:require("./../assets/img/1561458_7f3b-272x161.jpg"),
                    development: "design",
                    description: "CSS The Complete Guide 2020 (incl. Flexbox, Grid & Sass)",
                    sale: "$199.99",
                    price: "$100", 
                    vote: 5,
                },
                {
                    img:require("./../assets/img/1776542_30b1-272x161.jpg"),
                    development: "Google",
                    description: "Google Searching Ninja",
                    sale: "$69.99",
                    price: "$45", 
                    vote: 5,
                },
                {
                    img:require("./../assets/img/1208228_d61c_4-272x161.jpg"),
                    development: "Design",
                    description: "Digitally Painting Ligth and Color: Amateur to Master",
                    sale: "$139.99",
                    price: "$75", 
                    vote: 4,
                },
                {
                    img:require("./../assets/img/186792_41e4_4-272x161.jpg"),
                    development: "Arts & Craft",
                    description: "Become an Arabic Calligraphy Artist From Scratch",
                    sale: "$109.99",
                    price: "$95", 
                    vote: 5,
                },
                {
                    img:require("./../assets/img/366802_6fcc-272x161.jpg"),
                    development: "Food & Beverage",
                    description: "Get Wine Smart",
                    sale: "$49.99",
                    price: "$25", 
                    vote: 5,
                },
                {
                    img:require("./../assets/img/838056_611a_3-272x161.jpg"),
                    development: "Arts & Crafts",
                    description: "Paint Realistic Watercolour and Botanicals - MAGNOLIAS",
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
  
    .recent-courses-list{
        color: $venus;
        li{ 
            padding: 10px;
            &:hover,
            &.clicked{
                background-color: $mistic;
                border-radius: 20px;
                cursor: pointer;
            }
        }
    }

    .show-all{
        font-size: 0.8em;
        padding: 13px 36px;
    }

    .rigth-menu {
        position: absolute;
        top: 78%;
        right:13px;
        box-shadow: 4px 0px 22px 5px #888888;
    }
}

.subscribe {
    height: 20vh;
    background-color: $coral-red;
    font-size: 0.9em;
        button{
            background-color: $azure;
            color: white;
        }
}

.popular-courses{
    background-color: $mistic;
        button{
            padding: 5px 20px;
            font-size: 1.5em;
            color:  $mistic;
            border-color: $mistic;
            &:hover{
                background-color: $azure;
            }
        }
}

.work-with-us {
    img{
        width: 100%;
    }
    button{
        font-size: 0.8em;
        padding: 13px 36px;
        &:hover{
            background-color: $forest-green;
        }
    }
}

.investing{
    height: 80vh;
    background-image: url("./../assets/img/testimonial-1-1917x640-1-1914x639.jpg");
    background-size: cover;
    background-position: center;
    .cartoon{
        background-color: white;
        padding: 80px 70px;
        .sign{
            font-size: 0.8em;
        }
    }
    .triangle{    
    width: 0; 
    height: 0; 
    border-top: 20px solid transparent;
    border-bottom: 20px solid transparent;
    border-left: 20px solid white;
    }
}
</style>