.<template>
    <li class="col social">
        <div :class="network.color">
        <i :class="'fab '+ network.icon"></i>     
        </div>
    </li>
</template>

<script>
export default {
    name:"Social",
    props:["network"]
}
</script>

<style lang="scss">
@import "./../assets/scss/variables.scss";
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
</style>