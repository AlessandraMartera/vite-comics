<script >

export default {
    name: "AppHeader",
    Data() {
        return {


            links: [
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
                {
                    name: 'Character',
                    path: 'www.wikipedia.org'
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div>
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li v-for="link in links">
                    <a href="#">Character</a>
                </li>
                <li>
                    <a href="#">COMIX</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
                <li>
                    <a href="#">ciao</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style lang="scss">
@use '../styles/general.scss' as *;

header {
    height: 150px;
    background-color: #fff;
    display: flex;
    justify-content: space-around;

    img {
        margin-top: 20px;
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
        }

        a {
            text-decoration: none;
            color: #1c1c1c;
        }

        li:hover {
            border-bottom: 5px solid #307ef8;
        }
    }
}
</style>
