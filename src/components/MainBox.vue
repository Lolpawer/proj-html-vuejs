<template>
    <main>

        <jumbo-main
        :nav="nav"
        :button="button" />

        <delivery-main />

        <leaders-main
        :button="button" />

        <pricing-main />

    </main>
</template>

<script>
import DeliveryMain from './DeliveryMain.vue'
import JumboMain from './JumboMain.vue'
import LeadersMain from './LeadersMain.vue'
import PricingMain from './PricingMain.vue'

export default {
  components: {
    JumboMain,
    DeliveryMain,
    LeadersMain,
    PricingMain
  },
  props: {
      nav: Array,
      button: Object
  }
}
</script>

<style lang="scss" scoped>

</style>