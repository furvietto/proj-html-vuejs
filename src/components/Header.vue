.<template>
  <div class="container-fluid nav-bar">
      <div class="row">
          <!-- nav-bar-header -->
          <div class="col-12 nav-bar-header">      
              <div class="h-100 container">
                        <div class="h-100 row justify-content-between align-items-center">
                            <div class="col-2 language">
                                <span class="m-2">English</span>
                                <i class="fas fa-angle-down"></i>
                            </div>
                            <div class="col-7 h-100">
                                <div class="row h-100">
                                    <div class="col-8">
                                        <ul class=" list-unstyled row h-100 align-items-center justify-content-between">
                                            <Homepage v-for="(homepage,index) in homepages"
                                            :key="index"
                                            :col="homepage.col"
                                            :text="homepage.text"
                                            >
                                            </Homepage>
                                        </ul>
                                    </div>
                                    <div class="col-4">
                                        <ul class="list-unstyled  row h-100 align-items-center">
                                            <HomepageSocial v-for="(homepageSocial,index) in homepageSocials"
                                            :key="index" 
                                            :color="homepageSocial.color"
                                            :social="homepageSocial.social"
                                            >
                                            </HomepageSocial>
                                        </ul>
                                    </div>
                                </div>
                            </div>
                    </div>
                </div>      
          </div>
          <!-- /nav-bar-header -->

          <!-- navbar-middle -->
          <div class="col-12 nav-bar-middle">
              <div class="container h-100">
                  <div class="h-100 align-items-center row justify-content-between">
                      <div class="col">
                          <img src="./../assets/img/MasterStudy.svg" alt="">
                      </div>
                      <div class="col-4 category">
                          <i class="me-1 fas fa-bars"></i>
                          <span class="me-1">CATEGORY</span>
                          <!-- w-250 -->
                          <input class="input-search p-1 w-250" placeholder="Search course" type="text">
                          <!-- bottom-search -->
                          <span class="bottom-search text-white">
                              <i class="fas fa-search"></i>
                          </span>
                          
                      </div>
                      <div class="col">
                        <span class="instructor">
                            <i class="me-1 fas fa-bullhorn"></i>
                            <span class="me-3">Became an instructor</span>
                        </span>
                        <span class="enterprise">
                            <i class="me-1 fas fa-briefcase"></i>
                            <span>For Enterprise</span>
                        </span>
                      </div>
                      <div class="col">
                          <div class="row align-items-center justify-content-between">
                              <div class="col logIn">
                                  <i class="far fa-user"></i>
                                  <span>Log In</span>
                              </div>
                              <div class="col-6">
                                  <!-- sign-up -->
                                  <button type="button" class="sign-up rounded-pill btn btn-outline-danger">SIGN UP</button>
                              </div>
                              <div class="col">
                                  <i class="fs-4 far fa-bookmark"></i>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- navbar-middle -->

          <!-- navbar-bottom -->
          <div class="col-12 text-white nav-bar-bottom">
              <div class="container h-100">
                  <div class="h-100 row justify-content-center">
                      <div class="col-8">
                          <ul class="h-100 list-unstyled business align-items-center row justify-content-between">
                            <HomepageBusiness v-for="(business,index) in homepageBusiness"
                            :key="index"
                            :busi="business"
                            >
                            </HomepageBusiness>
                          </ul>
                      </div>
                  </div>
              </div>
          </div>
          <!-- /navbar-bottom -->
      </div>
  </div>
</template>

<script>
import Homepage from './Homepage.vue'
import HomepageSocial from "./HomepageSocial.vue"
import HomepageBusiness from './HomepageBusiness.vue'

export default {
    name:"Header",
    components:{
        Homepage,
        HomepageSocial,
        HomepageBusiness
    },
    data() {
        return {
            homepageBusiness:[
                {
                    icon:"fa-chart-line",
                    text:"Business",
                    col:"col"
                },
                {
                    icon:"fa-palette",
                    text:"Design",
                    col:"col"
                },
                {
                    icon:"fa-cog",
                    text:"Development",
                    col:"col"
                },
                {
                    icon:"fa-smile",
                    text:"Lifestyle",
                    col:"col"
                },
                {
                    icon:"fa-wallet",
                    text:"Office Productivity",
                    col:"col-3"
                },
            ],

            homepageSocials:[
                {
                    color:"facebook",
                    social:"fa-facebook"
                },
                {
                    color:"twitter",
                    social:"fa-twitter"
                },
                {
                    color:"instagram",
                    social:"fa-instagram"
                },
                {
                    color:"linkedin",
                    social:"fa-linkedin"
                },
                {
                    color:"google",
                    social:"fa-google-plus"
                },
                {
                    color:"youtube",
                    social:"fa-youtube"
                },
            ],
            homepages:[
                {
                    text:"Home",
                    col:"col"
                },
                {
                    text:"Pages",
                    col:"col"
                },
                {
                    text:"Course Formats",
                    col:"col-3"
                },
                {
                    text:"Courses",
                    col:"col"
                },
                {
                    text:"Formats",
                    col:"col"
                },
            ]
        }
    },
}
</script>

<style lang="scss">
@import "./../assets/scss/variables.scss";
.nav-bar {
    .nav-bar-header{
    font-size: 0.8em;
    color: $mistic;
    border-bottom: 1px solid $mistic;
    height: 5vh;
       
        .language{
            &:hover{
            color: $coral-red;
            cursor: pointer;
        }
      }             
    }
    .nav-bar-middle {
        font-size: 0.8em;
        height: 15vh;
        color: $venus;
        .logIn:hover,
        .enterprise:hover,
        .instructor:hover,
        .category:hover{
            color: $azure;
            cursor: pointer;
        }
        .w-250{
            width: 260px;
        }
        .input-search{
            background-color:$mistic ;
        }
        .bottom-search{
            background-color: $azure;
            padding: 7px 16px;
            cursor: pointer;
        }
        .sign-up {
          font-size: 0.9em;
          padding: 13px 36px;
        }
    }
    .nav-bar-bottom{
        height: 10vh ;
        background-color: $ebony-clay;
    }
}


</style>