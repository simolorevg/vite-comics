<script>
import AppBanner from './components/AppBanner.vue';
import AppContent from './components/AppContent.vue';
export default {
  components: {
    AppBanner,
    AppContent
  }

}
</script>

<template>
  <AppBanner />
  <AppContent />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
</style>
