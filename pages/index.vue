<template>
  <section class="container">
    <img src="~/static/map.png" alt="map of Stockholm"/>
    <div>
      <app-logo/>
      <h1 class="title">
        karta
      </h1>
      <h2 class="subtitle">
        Explore the world
      </h2>
      <div class="links">
        <a
          href="/map"
          class="button--green">Enter</a>
        <a
          href="https://github.com/Eleonore9/karta"
          target="_blank"
          class="button--grey">GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;


}

.container img {
  position: absolute;
  opacity: 0.6;
  z-index: -1;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
  z-index: 1;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
