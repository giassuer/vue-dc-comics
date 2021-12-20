<template>
  <div id="app">
    <Header />

    <main>

    </main>

    <FooterTop /> 

   <Footer />    
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import FooterTop from "./components/FooterTop.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    FooterTop,
    Footer,
  },
};
</script>

<style leng="scss">
@import './style/common.scss';
</style>
