<template>
  <div>
    <Header />
    <Navbar />
    <div class="container">
      <Menu />
      <Main />
      <div class="cart-article">
        <Cart />
        <Article />
      </div>
    </div>
  </div>
</template>

<script>
import Header from './Header.vue';
import Menu from './Menu.vue';
import Navbar from './Navbar.vue';
import Main from './Main.vue';
import Cart from './Cart.vue';
import Article from './Article.vue';

export default {
  name: 'UserLayout',
  components: {
    Header,
    Menu,
    Navbar,
    Main,
    Cart,
    Article
  }
}
</script>

<style scoped>
.container {
  display: flex;
}
.cart-article {
  display: flex;
  flex-direction: column;
}
nav {
  width: 200px;
}
main {
  flex: 1;
}
</style>
