<script >
import AppNavbar from "./components/AppNavbar.vue"
import AppHeader from "./components/AppHeader.vue"
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
    AppHeader,
    AppMain,
    AppFooter,
    AppFooterNav
  }
}
</script>

<template>
  <AppNavbar></AppNavbar>
  <AppHeader></AppHeader>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
  <AppFooterNav></AppFooterNav>
</template>

<style lang="scss" scoped></style>
