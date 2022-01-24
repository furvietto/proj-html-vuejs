.<template>
  <div class="container-fluid nav-bar">
      <div class="row">
          <!-- nav-bar-header -->
          <div class="col-12 nav-bar-header">      
              <div class="h-100 container">
                        <div class="h-100 row justify-content-between align-items-center">
                            <div class="col-2">
                                <span class="m-2">English</span>
                                <i class="fas fa-angle-down"></i>
                            </div>
                            <div class="col-7 h-100">
                                <div class="row h-100">
                                    <div class="col-8">
                                        <div class="row h-100 align-items-center justify-content-between">
                                            <div class="col">Home</div>
                                            <div class="col">Pages</div>
                                            <div class="col-4">Course Formats</div>
                                            <div class="col">Courses</div>
                                            <div class="col">Demos</div>
                                        </div>
                                    </div>
                                    <div class="col-4">
                                        <div class="row h-100 align-items-center">
                                            <div class="col">
                                            <i class="fab fa-facebook"></i>
                                            </div>
                                            <div class="col">
                                            <i class="fab fa-twitter"></i>
                                            </div>
                                            <div class="col">
                                            <i class="fab fa-instagram"></i>
                                            </div>
                                            <div class="col">
                                            <i class="fab fa-linkedin"></i>
                                            </div>
                                            <div class="col">
                                            <i class="fab fa-google-plus"></i>
                                            </div>
                                            <div class="col">
                                            <i class="fab fa-youtube"></i>
                                            </div>
                                        </div>
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
                      <div class="col-4">
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
                          <i class="me-1 fas fa-bullhorn"></i>
                          <span class="me-3">Became an instructor</span>
                          <i class="me-1 fas fa-briefcase"></i>
                          <span>For Enterprise</span>
                      </div>
                      <div class="col">
                          <div class="row align-items-center justify-content-between">
                              <div class="col">
                                  <i class="far fa-user"></i>
                                  <span>Log In</span>
                              </div>
                              <div class="col-6">
                                  <!-- sign-up -->
                                  <button type="button" class="sign-up rounded-pill btn btn-danger">SIGN UP</button>
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
                          <div class="h-100 align-items-center row justify-content-between">
                              <div class="col">
                                  <i class="me-2 fas fa-chart-line"></i>
                                  <span>Business</span>
                              </div>
                              <div class="col">
                                  <i class="me-2 fas fa-palette"></i>
                                  <span>Design</span>
                              </div>
                              <div class="col">
                                  <i class="me-2 fas fa-cog"></i>
                                  <span>Development</span>
                              </div>
                              <div class="col">
                                  <i class=" me-2 far fa-smile"></i>
                                  <span>Lifestyle</span>
                              </div>
                              <div class="col-3">
                                  <i class="me-2 fas fa-wallet"></i>
                                  <span>Office Productivity</span>
                              </div>
                          </div>
                      </div>
                  </div>
              </div>
          </div>
          <!-- /navbar-bottom -->
      </div>
  </div>
</template>

<script>
export default {
    name:"Header"
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
    }
    .nav-bar-middle {
        font-size: 0.8em;
        height: 15vh;
        color: $venus;
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