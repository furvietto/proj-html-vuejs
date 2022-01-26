.<template>
  <footer>
    <!-- contacts -->
    <div class="contacts container-fluid">
      <div class="row border-bottom pt-5 pb-5  justify-content-center">
        <div class="col-8 text-white">
          <div class="row gap-3 justify-content-between">
            <div class="col">
              <h5>ABOUT</h5>
              <p class="fs-08">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo asperiores ad rerum? Commodi dignissimos vero qui molestiae velit alias assumenda quisquam molestias lorem.</p>
            </div>
            <div class="col">
              <h5>CONTACT</h5>
              <div class="fs-08">
                <div class="mb-3">USA, California 20, First Avenue, California</div>
                <div>Tel: +1 212 458 300 32</div>
                <div class="mb-3">Fax: +1 212 375 24 14</div>
                <div class="e-mail">info@masterstudy.com</div>
              </div>              
            </div>
            <!-- social -->
            <div class="col">
              <h5>SOCIAL NETWORK</h5>
              <ul class="list-unstyled row gy-3 row-cols-4">
                <Social 
                v-for="(social,index) in socials"
                :key="index"
                :network="social"
                />
              </ul>
            </div>
            <!-- /social -->
            <div class="col">
              <img class="w-100" src="./../assets/img/Top-udemy-courses-90-percent-off.jpg" alt="">
            </div>
          </div>
        </div>
      </div>
      <div class="row copyrigth text-white pt-3 pb-3 justify-content-center">
        <div class="col-8">
          <img class="me-3" src="./../assets/img/footer-logo2x-50x56.png" alt="">
          <span>Copyrigth &#169; 2020</span>
          <a class="text-white ms-2 me-2" href="">Masterstudy</a>
          <span>Theme by</span>
          <a class="text-white ms-2" href="">StyleMixThemes</a>
        </div>
      </div>
    </div>
    <!-- contacts -->
  </footer>
</template>

<script>
import Social from './Social'

export default {
    name:"Footer",
    components:{
      Social
    },
    data() {
      return {
        socials:[
          {
            color:"facebook",
            icon:"fa-facebook"
          },
          {
            color:"instangram",
            icon:"fa-instagram"
          },
          {
            color:"linkedin",
            icon:"fa-linkedin"
          },
          {
            color:"pinterest",
            icon:"fa-pinterest"
          },
          {
            color:"twitter",
            icon:"fa-twitter"
          },
          {
            color:"dribble",
            icon:"fa-dribbble"
          },
          {
            color:"google",
            icon:"fa-google-plus"
          },
          {
            color:"skype",
            icon:"fa-skype"
          },
        ]
      }
    },
}
</script>

<style lang="scss">
@import "./../assets/scss/variables.scss";
.contacts{
  background-color: $oxford-blue;
  
  .fs-08{
    font-size: 0.8em;
  }
  .e-mail{
    color: $venus;
  }
}

.copyrigth {
  img{
    width: 20px;
  }
}
</style>