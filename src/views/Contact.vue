<template lang="html">
  <div class="container">
    <div class="columns">
      <div class="column">
        <h1 class="title">Contacto</h1>
      </div>
    </div>
    <div class="columns">
      <div class="column">
        <div class="card">
          <div class="card-content">
            <div class="media">
              <div class="media-left">
                <figure class="image is-128x128">
                  <img
                    src="../assets/profile.jpg"
                    alt="Placeholder image"
                    class="is-rounded"
                  />
                </figure>
              </div>
              <div class="media-content">
                <p class="title is-4">Jesus Cova</p>
                <p class="subtitle">jesuscovam@gmail.com</p>
                <p>+52 1 984 146 6416</p>
              </div>
            </div>

            <div class="content">
              Jesus Cova es un tecnico en informática, estudiante de
              mercadotecnia, y entusiasta del front-end.
              <br />
              <div class="icons">
                <a
                  v-for="icon in icons"
                  :key="icon.id"
                  :href="icon.href"
                  target="_newblank"
                >
                  <b-icon
                    type="is-primary"
                    size="is-medium"
                    :icon="icon.icon"
                  ></b-icon>
                </a>
              </div>
              <time datetime="2019-8-30">2019</time>
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
      icons: [
        { icon: "github-circle", href: "https://www.github.com/jesuscovam" },
        { icon: "twitter-circle", href: "https://www.twitter.com/jesusacova" }
      ]
    };
  }
};
</script>

<style lang="css" scoped></style>
