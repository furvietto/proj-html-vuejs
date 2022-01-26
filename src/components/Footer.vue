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
            <div class="col">
              <h5>SOCIAL NETWORK</h5>
              <div class="row gy-3 row-cols-4">
                <div class="col social">
                  <div class="facebook">
                    <i class="fab fa-facebook"></i>     
                  </div>
                </div>
                <div class="col social">
                  <div class="instangram">
                  <i class="fab fa-instagram"></i>
                  </div>
                </div>
                <div class="col social">
                  <div class="linkedin">
                  <i class="fab fa-linkedin"></i>
                  </div>
                </div>
                <div class="col social">
                  <div class="pinterest">
                  <i class="fab fa-pinterest"></i>
                  </div>
                </div>
                <div class="col social">
                  <div class="twitter">
                  <i class="fab fa-twitter"></i>
                  </div>
                </div>
                <div class="col social">
                  <div class="dribble">
                  <i class="fab fa-dribbble"></i>
                  </div>
                </div>
                <div class="col social">
                  <div class="google">
                  <i class="fab fa-google-plus"></i>
                  </div>
                </div>
                <div class="col social">
                  <div class="skype">
                  <i class="fab fa-skype"></i>
                  </div>
                </div>
              </div>
            </div>
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
export default {
    name:"Footer"
}
</script>

<style lang="scss">
@import "./../assets/scss/variables.scss";
.contacts{
  background-color: $oxford-blue;
  .social div{
      padding: 6px 11px;
      border-radius: 30px;
      &.facebook{
        background-color: $azure;
      }
      &.instangram{
        background-color: #c32aa3;
      }
      &.linkedin{
        background-color: $boston-blue;
      }
      &.pinterest{
        background-color: $amaranth;
      }
      &.twitter{
        background-color: #1da1f2;
      }
      &.dribble{
        background-color: $sundown;
      }
      &.google{
        background-color: $coral-red;
      }
      &.skype{
        background-color: $half-baked;
      }

  }
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