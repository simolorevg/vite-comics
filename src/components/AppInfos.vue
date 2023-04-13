<script>
export default {
    data() {
        return {
            dcComicsArray: [
                {
                    text: 'Characters',
                    link: '#char',
                    active: false
                },
                {
                    text: 'Comics',
                    link: '#comics',
                    active: false
                },
                {
                    text: 'Movies',
                    link: '#movies',
                    active: false
                },
                {
                    text: 'TV',
                    link: '#tv',
                    active: false
                },
                {
                    text: 'Games',
                    link: '#games',
                    active: false
                },
                {
                    text: 'Videos',
                    link: '#videos',
                    active: false
                },
                {
                    text: 'NEWS',
                    link: '#news',
                    active: false
                }
            ],
            shopArray: [
                {
                    text: 'Shop DC',
                    link: '#shopdc',
                    active: false
                },
                {
                    text: 'Shop DC Collectibles',
                    link: '#dccollectibles',
                    active: false
                }
            ],
            termArray: [
                {
                    text: 'Privacy',
                    link: '#privacy',
                    active: false
                },
                {
                    text: 'Terms Of Use',
                    link: '#tou',
                    active: false
                },
                {
                    text: 'Jobs',
                    link: '#jobs',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                },
                {
                    text: 'Contact Us',
                    link: '#contactus',
                    active: false
                }
            ],
            sitesArray: [
                {
                    text: 'Lorem',
                    link: '#lorem',
                    active: false
                },
                {
                    text: 'Lorem',
                    link: '#lorem',
                    active: false
                },
                {
                    text: 'Lorem',
                    link: '#lorem',
                    active: false
                }
            ]
        }
    }
}
</script>
<template>
    <div class="footer-container">
        <div class="infos-container">
            <div class="infos-links">
                <div class="first-row">
                    <div class="dc-comics-links">
                        <h3>DC COMICS</h3>
                        <ul v-for="item in dcComicsArray">
                            <li>
                                <a href="#link">
                                    {{ item.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div class="shop-links">
                        <h3>SHOP</h3>
                        <ul v-for="shopitem in shopArray">
                            <li>
                                <a href="#link">
                                    {{ shopitem.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="second-row">
                    <div class="term-of-use">
                        <h3>DC</h3>
                        <ul v-for="dcitem in termArray">
                            <li>
                                <a href="#link">
                                    {{ dcitem.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="third-row">
                    <div class="sites-links">
                        <h3>SITES</h3>
                        <ul v-for="sitem in sitesArray">
                            <li>
                                <a href="#link">
                                    {{ sitem.text }}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
            <div class="dc-bglogo">
                <img src="../assets/img/dc-logo-bg.png" alt="dc logo background">
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
@use '../style/general.scss' as *;
@use '../style/partials/mixins' as *;

.footer-container {
    width: 100%;
    background-image: url('../assets/img/footer-bg.jpg');

    .infos-container {
        width: 80%;
        margin: 0 auto;
        @include flexrwspacebtwcenter;

        .infos-links {
            width: 60%;
            @include flexrwaligncenter;

            h3 {
                color: white;
            }

            li {
                list-style: none;
            }

            a {
                text-decoration: none;
                color: grey;
            }

            .first-row {
                width: 20%;
                /*debug*/
                border: 1px solid white;
            }

            .second-row {
                width: 20%;
                @include flexclstart;
            }
        }

        .dc-bglogo {
            width: 40%;

            img {
                width: 100%;
            }
        }
    }
}
</style>