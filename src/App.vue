<template>
  <div id="app">
    <NavBar />
    <LandingPage/>
    <Content/>
    <DemoVideo/>
    <Footer/>
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import LandingPage from './components/LandingView.vue';
import Content from './components/Content.vue';
import DemoVideo from './components/DemoVideo.vue';
import Footer from './components/Footer.vue';

export default {
  name: "App",
  components: {
    NavBar,
    LandingPage,
    Content,
    DemoVideo,
    Footer
  },
};
</script>

<style>
body {
  background-color: #070d0d;
  min-height: 100vh;
  height: 100vh;
}
</style>
