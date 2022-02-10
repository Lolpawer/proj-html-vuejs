<template>
    <main>

        <jumbo-main
        :nav="nav"
        :button="button" />

        <delivery-main />

        <leaders-main
        :button="button" />

        <pricing-main />

        <choose-us-main 
        :button="button" />

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
    companyInfo: Array
  }
}
</script>

<style lang="scss" scoped>

</style>