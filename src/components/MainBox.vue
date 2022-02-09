<template>
    <main>

        <jumbo-main
        :nav="nav"
        :button="button" />

        <delivery-main />

    </main>
</template>

<script>
import DeliveryMain from './DeliveryMain.vue'
import JumboMain from './JumboMain.vue'

export default {
  components: {
      JumboMain,
    DeliveryMain
  },
  props: {
      nav: Array,
      button: Object
  }
}
</script>

<style lang="scss" scoped>

</style>