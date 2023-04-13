<script>
import AppBanner from './components/AppBanner.vue';
import AppContent from './components/AppContent.vue';
import AppInfos from './components/AppInfos.vue';
import AppMerchBanner from './components/AppMerchBanner.vue';
export default {
  components: {
    AppBanner,
    AppContent,
    AppMerchBanner,
    AppInfos
  }

}
</script>

<template>
  <AppBanner />
  <AppContent />
  <AppMerchBanner />
  <AppInfos />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
</style>
