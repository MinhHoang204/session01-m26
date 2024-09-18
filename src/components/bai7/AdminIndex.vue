<template>
  <div>
    <Header />
    <div class="container">
      <Menu />
      <Main />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from './Header.vue';
import Menu from './Menu.vue';
import Main from './Main.vue';
import Footer from './Footer.vue';

export default {
  name: 'AdminIndex',
  components: {
    Header,
    Menu,
    Main,
    Footer
  }
}
</script>

<style scoped>
.container {
  display: flex;
}
nav {
  width: 200px;
}
main {
  flex: 1;
}
</style>
