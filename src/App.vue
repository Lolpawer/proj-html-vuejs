<template>
  <div id="app">

    <!-- Header -->
    <header-box 
    :companyInfo="companyInformation" />

    <!-- Main Content -->
    <main-box 
    :nav="nav"
    :button="buttonContent"
    :companyInfo="companyInformation" />

    <!-- Footer -->
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
      companyInformation: {
        days: "Mon - Sat",
        hours: "9:00 - 18:00",
        phoneNumber: "+1 (305) 1234-5678",
        email: "hello@example.com",
        location: "Main Avenue, 987"
      },
      nav: [
        {
          text: "HOME"
        },
        {
          text: "SERVICES"
        },
        {
          text: "ABOUT"
        },
        {
          text: "PRICING"
        }
      ],
      buttonContent: {
        contact: "GET IN TOUCH",
        information: "READ MORE",
        send: "SEND",
        location: "VIEW MAP"
      }
    }
  }
}
</script>

<style lang="scss">
@import "./style/mainstyle.scss"

</style>
