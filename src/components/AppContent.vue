<script>
export default {

}
</script>
<template>
    <div class="content-container">
        <div class="content">
            Content Goes Here
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use "../style/partials/mixins" as *;

.content-container {
    width: 100%;
    height: 80px;
    color: white;
    background-color: rgba($color: #2e2d2d, $alpha: 1.0);
    padding: 10px;
    @include flexrwcenter;

    .content {
        width: 80%;
        margin: 0 auto;
    }
}
</style>