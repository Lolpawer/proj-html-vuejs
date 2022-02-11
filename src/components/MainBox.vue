<template>
    <main>

      <!-- Jumbotron + Navbar -->
      <jumbo-main
      :nav="nav"
      :button="button" />

      <!-- First section: delivery options -->
      <delivery-main />

      <!-- Second section: industry leaders --> 
      <leaders-main
      :button="button" />

      <!-- Third section: pricing options -->
      <pricing-main />

      <!-- Fourth section: why choose us? -->
      <choose-us-main 
      :button="button" />

      <!-- Fifth section: message form + company contact information -->
      <form-main 
      :button="button"
      :info="companyInfo" />

    </main>
</template>

<script>
import ChooseUsMain from './ChooseUsMain.vue'
import DeliveryMain from './DeliveryMain.vue'
import FormMain from './FormMain.vue'
import JumboMain from './JumboMain.vue'
import LeadersMain from './LeadersMain.vue'
import PricingMain from './PricingMain.vue'

export default {
  components: {
    JumboMain,
    DeliveryMain,
    LeadersMain,
    PricingMain,
    ChooseUsMain,
    FormMain   
  },
  props: {
    nav: Array,
    button: Object,
    companyInfo: Object
  }
}
</script>

<style lang="scss" scoped>
</style>