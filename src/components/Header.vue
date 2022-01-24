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
                          <img src="./../assets/MasterStudy.svg" alt="">
                      </div>
                      <div class="col-4">
                          <i class="me-1 fas fa-bars"></i>
                          <span class="me-1">CATEGORY</span>
                          <input class="input-search p-1 w-50" placeholder="Search course" type="text">
                          <span class="bottom-search">
                              <i class="fas fa-search"></i>
                          </span>
                          
                      </div>
                      <div class="col">
                          <i class="fas fa-bullhorn"></i>
                          <span>Became an instructor</span>
                          <i class="fas fa-briefcase"></i>
                          <span>For Enterprise</span>
                      </div>
                      <div class="col">

                      </div>
                  </div>
              </div>
          </div>
          <!-- navbar-middle -->
      </div>
  </div>
</template>

<script>
export default {
    name:"Header"
}
</script>

<style lang="scss">
.nav-bar {
    font-size: 0.8em;
    .nav-bar-header{
    color: #dde6eb;
    border-bottom: 1px solid #dde6eb;
    height: 5vh;             
    }
    .nav-bar-middle {
        height: 10vh;
        color: #9b8a92;
        .input-search{
            background-color:#dde6eb ;
        }
        .bottom-search{
            background-color: #375ca2;
            padding: 7px 16px;
        }
    }
}


</style>