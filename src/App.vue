<template>
  <div id="app">
    <Header />

    <main>
      <ComicsList />
    </main>

    <FooterTop /> 
   <Footer />    
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import FooterTop from "./components/FooterTop.vue";
import Footer from "./components/Footer.vue";
import ComicsList from "./components/ComicsList.vue";

export default {
  name: "App",
  components: {
    Header,
    FooterTop,
    Footer,
    ComicsList,
  },
   
};
</script>

<style leng="scss">
@import './style/common.scss';

</style>
