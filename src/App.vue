<template>
  <div id="app">

    <Header :linksArray="links" :service="callService"/>
    <Jumbotron />
    <Main />
    <Footer />

  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
    Main,
    Footer
  },
  data: function() {
    return {
      links: [
        {
          text: 'Home',
          url: '#',
          dropDown: true
        },
        {
          text: 'Services',
          url: '#',
          dropDown: true
        },
        {
          text: 'Why Us',
          url: '#',
          dropDown: false
        },
        {
          text: 'Case Studies',
          url: '#',
          dropDown: false
        },
        {
          text: 'About',
          url: '#',
          dropDown: false
        },
        {
          text: 'Blog',
          url: '#',
          dropDown: false
        }
      ],
      callService: '(555) 802-1234',
    }
  },
};
</script>

<style lang="scss">
@import './style/generals';
@import './style/commons';

</style>
