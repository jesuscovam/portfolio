<template lang="html">
  <div class="container">
    <div class="columns">
      <div class="column center">
        <h1 class="subtitle">
          <strong>Error 404</strong>
          <vue-typer text=" página no encontrada🙇‍♀️ 🙇"></vue-typer>
        </h1>
      </div>
    </div>
  </div>
</template>

<script>
import { VueTyper } from "vue-typer";
export default {
  components: {
    VueTyper
  },
  data() {
    return {
      isShowing: false,
      bkClass: "bk",
      blurClass: "blur"
    };
  }
};
</script>

<style lang="css" scoped>
.center{
  text-align: center;
}

.fade-enter-active, .fade-leave-active {
  transition: opacity 0.25s ease-out;
}

.fade-enter, .fade-leave-to{
  opacity: 0
}

.bk{
  transition: all 0.1s ease-out;
}

.blur{
  filter: blur(2px);
  opacity: 0.4s;
}

.vue-typer{
  font-family: inherit;
}
</style>
