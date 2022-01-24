.<template>
  <div class="jumbotron container-fluid">
      <div class="row h-100">
          <div class="col-12 text-light back-jumbo position-relative">
            <img class="h-100 w-50" src="./../assets/slide-1.jpg" alt="">
            <div class="row h-100">
                <div class="col-6 h-100">
                    <div class="row h-100 align-items-center justify-content-end">
                        <div class="col-9">
                            <h1 class="mb-4">Udemy Affiliates Sales</h1>
                            <div class="fs-5">Monetize your audience and attract new customers with Udemy!</div>
                        </div>
                    </div>
                </div>
            </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Main"
}
</script>

<style lang="scss">
.jumbotron{
    height: 40vh;
    margin: 20px 0;
    .back-jumbo{
        background-image: linear-gradient(65deg, #ff4550, #ff4550 55%, transparent 50%);
        img{
            position: absolute;
            top: 0;
            right: 0;
            z-index:-1;
        }
    }
}
</style>