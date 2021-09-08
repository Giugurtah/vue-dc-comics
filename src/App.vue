<template>
  <div id="app">
    <Header />
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
export default {
  name: 'App',
  components: {
    Header,
    Main,
    FooterNav,
    FooterSocials
  }
}
</script>

<style lang="scss">
@import "@/assets/style/index.scss";
</style>
