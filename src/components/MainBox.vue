<template>
    <main>

        <jumbo-main
        :nav="nav"
        :button="button" />

    </main>
</template>

<script>
import JumboMain from './JumboMain.vue'

export default {
  components: {
      JumboMain
  },
  props: {
      nav: Array,
      button: Object
  }
}
</script>

<style lang="scss" scoped>

</style>