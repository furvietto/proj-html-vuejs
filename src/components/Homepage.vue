.<template>
  <li :class="col">
      {{text}}
  </li>
</template>

<script>
export default {
    name:"Homepage",
    props:["col","text"]
}
</script>

<style lang="scss" scoped>
    li{
      &:hover{
          color: red;
      }  
    }
</style>