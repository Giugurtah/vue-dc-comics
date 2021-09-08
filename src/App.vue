<template>
  <div id="app">
    <Header />
    <Jumbotron />
    <Main />
    <FooterNav />
    <FooterSocials />
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import FooterNav from './components/FooterNav.vue'
import FooterSocials from './components/FooterSocials.vue'
import Jumbotron from './components/Jumbotron.vue'
export default {
  name: 'App',
  components: {
    Header,
    Main,
    FooterNav,
    FooterSocials,
    Jumbotron
  }
}
</script>

<style lang="scss">
@import "@/assets/style/index.scss";
</style>
