<template>
  <div id="app">
  <Header></Header>
  <Main></Main>
  <Footer></Footer>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'

export default {
  name: "App",
  components: {
   Header,
   Main,
   Footer
  },
};
</script>

<style lang="scss" >
@import url('https://fonts.googleapis.com/css2?family=Corinthia:wght@400;700&family=Montserrat:wght@100;200;300;400;500;600;700;800;900&family=Open+Sans:wght@300;400;500;600;700;800&display=swap');
 @import "~bootstrap/scss/bootstrap";

html {
font-family: 'Open Sans', sans-serif;
}
</style>
