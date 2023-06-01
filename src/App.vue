<script >
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppProductList from './components/AppProductList.vue';
export default {
  components: {
    AppHeader,
    AppFooter,
    AppProductList
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <section id="jumbotron"></section>
    <section>
      <AppProductList />
    </section>
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/variables.scss' as *;
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600&family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,400&display=swap');

* {
  font-family: 'Montserrat',
    sans-serif;
  font-family: 'Ubuntu',
    sans-serif;
  font-weight: 500;
}

#jumbotron {
  width: 100%;
  height: 400px;
  background-image: url(./assets/img/jumbotron.jpg);
  background-size: cover;
}

main {
  color: #fff;
}
</style>
