<template lang="html">
  <b-navbar>
    <template slot="brand">
      <b-navbar-item tag="router-link" to="/" class="logo">
        Jesus Cova
      </b-navbar-item>
    </template>
    <template slot="end">
      <b-navbar-item tag="router-link" to="/portfolio">
        <button class="button is-primary">Portfolio</button>
      </b-navbar-item>
      <b-navbar-item tag="router-link" to="/contacto">
        <button class="button is-light">Contacto</button>
      </b-navbar-item>
    </template>
  </b-navbar>
</template>

<script>
export default {};
</script>

<style lang="css" scoped></style>
