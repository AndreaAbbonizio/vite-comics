<script >
import AppNavbar from "./components/AppNavbar.vue"
import AppJumbotron from "./components/AppJumbotron.vue"
import AppListFilm from "./components/AppListFilm.vue"
import AppMain from "./components/AppMain.vue"
import AppFooter from "./components/AppFooter.vue"
import AppFooterNav from "./components/AppFooterNav.vue"
export default {
  data() {
    return {

    }
  },
  components: {
    AppNavbar,
    AppJumbotron,
    AppListFilm,
    AppMain,
    AppFooter,
    AppFooterNav
  }
}
</script>

<template>
  <AppNavbar></AppNavbar>
  <AppJumbotron></AppJumbotron>
  <AppListFilm></AppListFilm>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
  <AppFooterNav></AppFooterNav>
</template>

<style lang="scss" scoped></style>
