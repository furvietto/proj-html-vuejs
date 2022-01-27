.<template>
    <li :class="'col'+' '+ color ">
        <i :class="'fab'+' '+ social"></i>
    </li>
</template>

<script>
export default {
    name:"HomepageSocial",
    props:["color","social"]
}
</script>

<style lang="scss" scoped>
@import "./../assets/scss/variables.scss";
    .facebook:hover{
        color: $azure;
    }
    .twitter:hover{
        color: #1da1f2;
    }
    .instagram:hover{
        color:  #c32aa3;
    }
    .linkedin:hover{
        color:  $boston-blue;
    }
    .google:hover{
        color: $coral-red;
    }
    .youtube:hover{
        color: $amaranth;
    }
</style>