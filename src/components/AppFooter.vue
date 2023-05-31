<script >

export default {
    name: "AppFooter",
    data() {
        return {
            navLinks: ['DIGITALS COMICS', 'DC MERCHANDISE', 'SUBSCRIPTION', 'COMIC SHOP LOCATOR', 'DC POWER VISA']
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
                    <li v-for="navLink in navLinks">
                        {{ navLink }}
                    </li>
                </ul>
            </div>

        </nav>
        <!-- content uls links -->
        <div id="footer_content">
        </div>
        <!-- button section -->
        <div id="buttons_footer">
            <div class="wrapper">
                <button>
                    SIGN-UP NOW!
                </button>

                <div class="incos_links">
                    follow us: fb tw yt pin maps
                </div>
            </div>

        </div>
    </footer>
</template>

<style lang="scss">
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

        .wrapper {}
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
        }



    }
}
</style>
