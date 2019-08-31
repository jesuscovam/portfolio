<template>
  <div id="app">
    <Navbar />
    <transition name="comps">
      <router-view />
    </transition>
    <Footer />
  </div>
</template>
<script>
import Navbar from "./components/Navbar";
import Footer from "./components/Footer";
export default {
  components: {
    Navbar,
    Footer
  }
};
</script>
<style scoped>
.comps-enter-active,
.comps-leave-active {
  transition: opacity 0.5s;
}

.comps-enter,
.comps-leave-to {
  opacity: 0;
}
</style>
