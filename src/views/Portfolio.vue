<template lang="html">
  <div class="container">
    <div class="columns is-center">
      <div class="column">
        <h2 class="title ">Portfolio🗂</h2>
      </div>
    </div>
    <div class="columns">
      <div class="column" v-for="(muestra, index) in muestras" :key="index">
        <div class="card">
          <div class="card-image">
            <figure class="image is4by3">
              <img :src="muestra.img" :alt="muestra.name" class="img-card" />
            </figure>
          </div>
          <div class="card-content">
            <div class="media">
              <div class="media-content is-center">
                <button
                  class="button is-primary"
                  :href="muestra.href"
                  target="_newblank"
                >
                  {{ muestra.name }}
                </button>
              </div>
            </div>
            <div class="content">
              {{ muestra.content }}
              <br />
              <br />

              <h4 class="subtitle">Tooling:</h4>
              <ul class="tool-list">
                <li v-for="tool in muestra.tools" :key="tool.id">
                  {{ tool }}
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      muestras: [
        {
          name: "bscambio.com",
          href: "https://www.bscambio.com",
          img: require("../assets/bscambio.png"),
          content:
            "Pagina web que muestra el tipo de cambio de bolivares actual",
          tools: ["react", "gatsby", "material-ui"]
        },
        {
          name: "demo bootstrap",
          href: "https://bootsy101-jesus.netlify.com/",
          img: require("../assets/bootsy2.png"),
          content: "Demo de bootstrap con iconos",
          tools: ["vue", "bootstrap"]
        },
        {
          name: "login con firebase",
          href: "https://login-jesus.netlify.com/",
          img: require("../assets/login.png"),
          content: "Login de pagina web con vuetify y firebase",
          tools: ["vue", "firebase", "vuetify"]
        }
      ]
    };
  }
};
</script>

<style lang="css" scoped>
.is-center {
  text-align: center;
}

.img-card{
  height: 200px;
  width: 350px;
  margin: auto;
}
.tool-list{
  list-style: none;
}
</style>
