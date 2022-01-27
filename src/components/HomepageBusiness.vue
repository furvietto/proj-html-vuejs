.<template>
    <li
    :class="busi.col+' '+ 'h-100 d-flex justify-content-center align-items-center'">
        <i :class="'me-2 fas'+' '+ busi.icon"></i>
        <span>{{busi.text}}</span>
    </li>
</template>

<script>
export default {
    name:"HomepageBusiness",
    props:["busi"]
}
</script>

<style lang="scss" scoped>
@import "./../assets/scss/variables.scss";
    li:hover{
            background-color: $coral-red;
            transition: all 0.7s;
            }
</style>