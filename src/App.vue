<template>
  <div id="app">
    <header-box 
    :days="companyDays"
    :hours="companyHours"
    :number="companyNumber"
    :email="companyEmail" />
    <main-box />
    <footer-box />
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import MainBox from './components/MainBox.vue'
import FooterBox from './components/FooterBox.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    MainBox,
    FooterBox
  },
  data() {
    return {
      companyDays: "Mon - Sat",
      companyHours: "9:00 - 18:00",
      companyNumber: "+1 (305) 1234-5678",
      companyEmail: "hello@example.com"
    }
  }
}
</script>

<style lang="scss">
@import "./style/mainstyle.scss"

</style>
