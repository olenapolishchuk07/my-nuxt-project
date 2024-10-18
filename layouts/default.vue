<template>
  <div class="container">
    <Header />
    <div class="content">
      <Menu />
      <Main />
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from '~/components/Header.vue';
import Menu from '~/components/Menu.vue';
import Main from '~/components/Main.vue';
import Footer from '~/components/Footer.vue';

export default {
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
  flex-direction: column;
  height: 100vh;
}

.content {
  display: flex;
  flex-grow: 1;
}

Menu {
  flex: 0 0 40%;
  background-color: #e9ecef;
}

Main {
  flex: 0 0 60%;
  padding: 20px;
}

.header, .footer {
  background-color: #808080;
  color: white;
  text-align: center;
  padding: 10px 0;
}

.main {
  padding: 20px;
}

.menu {
  padding: 20px;
  background-color: #f8f9fa;
}
</style>
