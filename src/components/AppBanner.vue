<script>
export default {
    data() {
        return {
            links: [
                {
                    text: 'CHARACTERS',
                    link: '#characters',
                    active: false
                },
                {
                    text: 'COMICS',
                    link: '#comics',
                    active: false
                },
                {
                    text: 'MOVIES',
                    link: '#movies',
                    active: false
                },
                {
                    text: 'TV',
                    link: '#tv',
                    active: false
                },
                {
                    text: 'GAMES',
                    link: '#games',
                    active: false
                },
                {
                    text: 'COLLECTIBLES',
                    link: '#collectibles',
                    active: false
                },
                {
                    text: 'VIDEOS',
                    link: '#videos',
                    active: false
                },
                {
                    text: 'FANS',
                    link: '#fans',
                    active: false
                },
                {
                    text: 'NEWS',
                    link: '#news',
                    active: false
                },
                {
                    text: 'SHOP',
                    link: '#shop',
                    active: false
                }
            ],
            title: 'hello'
        }
    }
}
</script>
<template>
    <div class="banner">
        <div class="banner-container">
            <div class="logo-section"><img src="../assets/img/dc-logo.png" alt="dc-logo"></div>
            <div class="links-section" v-for="item, index in links">
                <ul>{{ item.text }}</ul>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use "../style/general.scss" as *;
@use "../style/partials/mixins" as *;

.banner {
    width: 100%;
    background-color: white;
    margin-top: 10px;
    @include flexrwcenter;

    .banner-container {
        width: 80%;
        height: 90px;
        @include flexrwcenter;

        img {
            max-width: 100%;
            max-height: 100%;
        }

        .logo-section {
            width: 30%;
            height: 100%;
            padding: 10px;
        }

        .links-section {
            flex-grow: 1;
            height: 100%;
            @include flexrwcenter;

            &:hover {
                border-bottom: 2px solid aqua;
            }
        }
    }
}
</style>