<script >

export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'COMIX',
                    path: 'www.google.com'
                },
                {
                    name: 'MOVIE',
                    path: 'www.google.com'
                },
                {
                    name: 'TV',
                    path: 'www.google.com'
                },
                {
                    name: 'GAMES',
                    path: 'www.google.com'
                },
                {
                    name: 'COLLECTIBLES',
                    path: 'www.google.com'
                },
                {
                    name: 'VIDEOS',
                    path: 'www.google.com'
                },
                {
                    name: 'FANS',
                    path: 'www.google.com'
                },
                {
                    name: 'NEWS',
                    path: 'www.google.com'
                },
                {
                    name: 'SHOP',
                    path: 'www.google.com'
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div class="wrapper">
            <div id="logo">
                <img src="../assets/img/dc-logo.png" alt="">
            </div>

            <nav>
                <ul>
                    <li v-for="link in links">
                        <a href="#">{{ link.name }}</a>
                    </li>
                </ul>
            </nav>
        </div>

    </header>
</template>

<style lang="scss">
@use '../styles/general.scss' as *;
@use '../styles/variables.scss' as *;

header {
    background-color: #fff;

    .wrapper {
        height: 150px;

        display: flex;
        justify-content: space-around;

        #logo {
            padding: 20px;
        }


        ul {
            height: 100%;
            display: flex;
            gap: 5px;
            align-items: center;

            li {
                height: 100%;
                display: flex;
                align-items: center;
                margin-left: 5px;
            }

            a {
                display: flex;
                align-items: center;
                height: 100%;
                text-decoration: none;
                font-size: 20px;
                color: #1c1c1c;
            }

            a:hover {
                border-bottom: 5px solid $primary;
                color: $primary;
            }
        }
    }
}
</style>
