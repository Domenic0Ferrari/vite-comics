<script>
import ComicHeader from './components/ComicHeader.vue'
import ComicMain from './components/ComicMain.vue'
import ComicFooter from './components/ComicFooter.vue'
export default {
  components: {
    ComicHeader,
    ComicMain,
    ComicFooter
  }
}
</script>

<template>
  <ComicHeader />
  <ComicMain />
  <ComicFooter />
</template>

<style lang="scss">
@use './assets/style/general.scss' as *;
</style>
