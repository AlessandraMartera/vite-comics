<script >

export default {
    name: "AppHeader"
}
</script>

<template>
    <header>
        <div>
            Logo
        </div>
        <nav>
            <ul>
                <li>
                    <a href="#">Characters</a>
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
    padding: 20px 10px;
    display: flex;
    justify-content: space-around;
}
</style>
