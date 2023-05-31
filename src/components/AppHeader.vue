<script >

export default {
    name: "AppHeader",
    Data() {
        return {
            links: [
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
                {
                    name: 'CHARACTERS',
                    path: 'www.google.com'
                },
            ]
        }
    }
}
</script>

<template>
    <header>
        <div id="logo">
            <img src="../assets/img/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li v-for="link in links">
                    <a href="#">{{ link.name }}</a>
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
        }

        a {
            display: flex;
            align-items: center;
            height: 100%;
            text-decoration: none;
            color: #1c1c1c;
        }

        a:hover {
            border-bottom: 5px solid #307ef8;
            color: #307ef8;
        }
    }
}
</style>
