<script>
import AppBanner from './components/AppBanner.vue';
import AppContent from './components/AppContent.vue';
import AppInfos from './components/AppInfos.vue';
import JumboComic from './components/JumboComic.vue';
export default {
  components: {
    AppBanner,
    AppContent,
    AppInfos,
    JumboComic
  }
}
</script>

<template>
  <AppBanner />
  <JumboComic />
  <AppContent />
  <AppInfos />
</template>

<style lang="scss">
@use "./style/general.scss" as *;
</style>
