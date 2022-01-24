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
          <div class="p-0 col fs-5 fw-bold">
              Popular Development Courses
          </div>
      </div>
      <ul class="row gap-3 list-unstyled">
          <li class="p-0 col card">           
              <img  src="./../assets/img/895786_7b4b_2-272x161.jpg" alt="">
              <div class="card-body">
                    <div class="development">
                        Development <i class="fas fa-angle-right"></i>
                    </div>
                    <div class="description">
                        The Complete iOS 10 &amp; Swift 3 Developer Course
                    </div>
                    <div class="row align-items-center">
                        <div class="col">
                            <img src="./../assets/img/starfull.svg" alt="">
                            <img src="./../assets/img/starfull.svg" alt="">
                            <img src="./../assets/img/starfull.svg" alt="">
                            <img src="./../assets/img/starfull.svg" alt="">
                            <img src="./../assets/img/staremptyl.svg" alt="">
                        </div>
                        <div class="col">
                            <div class="sale">
                                <del>
                                     $199.99
                                </del>                           
                            </div>
                            <div>
                                <strong>
                                      $100
                                </strong>                          
                            </div>
                        </div>
                    </div>
              </div>
          </li>
          <li class="col card"></li>
          <li class="col card"></li>
          <li class="col card"></li>
          <li class="col card"></li>
      </ul>
  </div>
  <!-- popular courses -->
</main>
  
</template>

<script>
export default {
    name:"Main"
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
    height: 40vh;
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
</style>