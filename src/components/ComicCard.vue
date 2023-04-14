<script>
export default {
    name: 'ComicCard',
    props: {
        thumb: String,
        series: String,
        type: String
    }
}
</script>
<template>
    <div class="comic-card">
        <div class="comic-img">
            <img :src="thumb" alt="">
        </div>
        <div class="comic-text">
            {{ type }}
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/partials/mixins' as *;


.comic-card {
    width: calc(100% / 6 - 20px);
    height: 200px;
    border: 1px solid yellow;
    @include flexclcenter;


    .comic-img {
        width: 100%;
        height: 60%;
        border: 1px solid red;

        img {
            max-width: 100%;
            object-fit: cover;
            height: 100%;
        }
    }

    .comic-text {
        flex-grow: 1;
        width: 100%;
        background-color: orange;
        color: black;
    }
}
</style>