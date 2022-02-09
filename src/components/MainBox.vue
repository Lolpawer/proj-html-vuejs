<template>
    <main>

        <jumbo-main
        :nav="nav" />

    </main>
</template>

<script>
import JumboMain from './JumboMain.vue'

export default {
  components: {
      JumboMain
  },
  props: {
      nav: Array
  }
}
</script>

<style lang="scss" scoped>

</style>