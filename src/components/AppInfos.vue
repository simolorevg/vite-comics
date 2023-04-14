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
        <div class="merch-container">
            <div class="merch-selection">
                <div class="buy-thing">
                    <div class="thing-icon">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
                    </div>
                    <div class="thing-text">
                        <p>Lorem Thing</p>
                    </div>
                </div>
                <div class="buy-thing">
                    <div class="thing-icon">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                    </div>
                    <div class="thing-text">
                        <p>Lorem Thing</p>
                    </div>
                </div>
                <div class="buy-thing">
                    <div class="thing-icon">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                    </div>
                    <div class="thing-text">
                        <p>Lorem Thing</p>
                    </div>
                </div>
                <div class="buy-thing">
                    <div class="thing-icon">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
                    </div>
                    <div class="thing-text">
                        <p>Lorem Thing</p>
                    </div>
                </div>
                <div class="buy-thing">
                    <div class="thing-icon">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                    </div>
                    <div class="thing-text">
                        <p>Lorem Thing</p>
                    </div>
                </div>
            </div>
        </div>
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
        <div class="call-to-action">
            <div class="container-to-action">
                <a href="#link" class="sign-up-btn">
                    SIGN UP NOW
                </a>
                <div class="social-links">
                    <h3>Follow Us</h3>
                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">
                </div>
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
    position: relative;

    .merch-container {
        background-color: #0082f8;
        width: 100%;
        position: absolute;

        .merch-selection {
            width: 70%;
            margin: 0 auto;
            @include flexrwcenter;

            .buy-thing {
                width: calc(100% / 5);
                display: flex;
                padding: 5px;
                cursor: pointer;

                .thing-icon {
                    width: 40%;
                    margin-left: 10px;

                    img {
                        max-width: 50px;
                    }
                }

                .thing-text {
                    flex-grow: 1;
                }

                .thing-text {
                    @include flexrwcenter;
                    color: white;
                }
            }
        }
    }

    .infos-container {
        width: 80%;
        margin: 0 auto;
        @include flexrwspacebtwcenter;

        .infos-links {
            width: 60%;
            display: flex;

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
            }

            .second-row {
                width: 20%;
            }

            .third-row {
                width: 20%;
                height: 100%;
            }
        }

        .dc-bglogo {
            width: 40%;

            img {
                width: 100%;
            }
        }
    }

    .call-to-action {
        width: 100%;
        height: 70px;
        background-color: black;
        position: absolute;
        bottom: 0;
        left: 0;
        color: white;

        .container-to-action {
            width: 80%;
            margin: 0 auto;
            @include flexrwspacebtwcenter;
            padding: 10px;

            a {
                color: white;
                text-decoration: none;
            }

            .sign-up-btn {
                border: 1px solid blue;
                width: 9em;
                height: 2em;
                @include flexrwcenter;
            }

            .social-links {
                height: 100%;
                @include flexrwcenter;

                h3 {
                    color: aqua;
                }
            }
        }
    }
}
</style>