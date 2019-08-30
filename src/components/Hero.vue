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
                Esta es una muestra de mis apps
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
export default {};
</script>

<style lang="css" scoped>
.text-center {
  text-align: center;
  margin-top: 50px;
}
</style>
