<script >

export default {
    name: "AppFooter",
    data() {
        return {
            navButtons: [
                {
                    text: 'DIGITALS COMICS',
                    immage: 'img/buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    immage: 'img/buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    immage: 'img/buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    immage: 'img/buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    immage: 'img/buy-dc-power-visa.svg'
                }
            ],
            icons: ['img/footer-facebook.png', 'img/footer-twitter.png', 'img/footer-youtube.png', 'img/footer-pinterest.png', 'img/footer-periscope.png']
        }
    }
}
</script>

<template>
    <footer>
        <!-- nav -->
        <nav>
            <div class="wrapper">
                <ul>
                    <li v-for="navButton in navButtons">

                        <img :src="navButton.immage" alt="">
                        {{ navButton.text }}
                    </li>
                </ul>
            </div>

        </nav>
        <!-- content uls links -->
        <div id="footer_content">
            <div class="wrapper">

                <div id="list">

                    <ul>
                        <li>
                            <h2>DC COMICS</h2>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>

                    <ul>
                        <li>
                            <h2>SHOP</h2>
                        </li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>

                    </ul>


                    <ul>
                        <li>
                            <h2>DC</h2>
                        </li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                        <li>Videos</li>
                        <li>Videos</li>
                        <li>Videos</li>
                        <li>Videos</li>
                    </ul>

                    <ul>
                        <li>
                            <h2>SITES</h2>
                        </li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>

                    </ul>
                </div>

                <div id="logo-bg">

                </div>
            </div>
        </div>

        <!-- button section -->
        <div id="buttons_footer">
            <div class="wrapper">
                <button>
                    SIGN-UP NOW!
                </button>

                <div class="incos_links">
                    <span>FOLLOW US: </span>

                    <ul>
                        <li v-for="elIcon in icons">
                            <img :src="elIcon" alt="">
                        </li>
                    </ul>

                </div>

            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/variables.scss' as *;

footer {
    height: 600px;
    color: #fff;

    #footer_content {
        height: calc(100% - 250px);
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
        background-repeat: no-repeat;

        .wrapper {
            height: 100%;
            display: flex;

            #list {
                width: 50%;
                padding: 25px;
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                gap: 5px;

                ul {
                    color: #777777;
                    font-weight: 100;
                    font-size: 14px;
                    margin: 10px;

                    li {
                        margin-bottom: 5px;
                    }

                    h2 {
                        color: #fff;
                        margin-bottom: 5px;
                    }
                }
            }

            #logo-bg {
                width: 50%;
                height: 100%;
                background-image: url(../assets/img/dc-logo-bg.png);
                background-size: cover;
                background-position: center;
                background-repeat: no-repeat;
            }
        }


    }

    nav {

        background-color: $primary;

        .wrapper {
            height: 150px;

            ul {
                height: 100%;
                display: flex;
                justify-content: space-around;

                li {
                    height: 100%;
                    display: flex;
                    align-items: center;

                    img {
                        width: 50px;
                        margin-right: 5px;
                    }
                }
            }
        }


    }

    #buttons_footer {

        background-color: #212121;

        .wrapper {
            height: 100px;
            display: flex;
            justify-content: space-between;
            align-items: center;

            button {
                cursor: pointer;
                color: #fff;
                background-color: #212121;
                padding: 15px;
                border: 2px solid $primary;
            }

            .incos_links {
                color: #777777;
                font-size: 20px;
                display: flex;
                align-items: center;
                gap: 15px;

                span {
                    color: $primary;
                    font-weight: 800;
                }

                ul {
                    display: flex;
                    gap: 8px;
                }
            }
        }
    }
}
</style>
