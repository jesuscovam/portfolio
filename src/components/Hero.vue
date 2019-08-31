<template lang="html">
  <div class="container">
    <div class="columns">
      <div class="column">
        <div class="hero">
          <div class="hero-body">
            <div class="container text-center">
              <h1 class="title">
                Hola👋
              </h1>

              <h2 class="subtitle">
                <vue-typer
                  text="Esta es una muestra de mis apps"
                  :repeat="0"
                ></vue-typer>
              </h2>
              <router-link to="/portfolio">
                <button class="button is-primary">Portfolio</button>
              </router-link>
            </div>
          </div>
        </div>
      </div>
      <div class="column">
        <figure class="image is-1by1">
          <img src="../assets/hero.png" />
        </figure>
      </div>
    </div>
  </div>
</template>

<script>
import { VueTyper } from "vue-typer";
export default {
  components: {
    VueTyper
  }
};
</script>

<style lang="css" scoped>
.text-center {
  text-align: center;
  margin-top: 50px;
}
.vue-typer{
  font-family: inherit;
  color: inherit;
}
</style>
