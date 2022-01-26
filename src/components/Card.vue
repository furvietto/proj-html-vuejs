.<template>
    <li class="py-2 col">
            <div class="p-0 h-100 card">
                <div class="scale">
                    <img class="ciao" :src="card.img" alt="">
                </div>
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
            </div>                   
          </li>
</template>

<script>
export default {
    name:"Card",
    props:["card"]
}
</script>

<style lang="scss">
 @import "./../assets/scss/variables.scss";
 li{
     cursor: pointer;
     .scale{
         overflow: hidden;
         & > img{
             width: 100%;
         }
     }
    &:hover .scale > img{
        transition: all 1s;
        transform: scale(1.1);
    }
     .development {
         font-size: 0.8em;
         margin-bottom: 10px;
         color: $venus;
     }
     .description {
         font-size: 0.8em;
         border-bottom: 1px solid black;
         padding-bottom: 15px;
     }
     .sale{
         font-size: 0.8em;
     }
 }
</style>