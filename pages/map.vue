<template>
  <section class="container">
    <div class="nav">
      <a href="/">
	<img src="~/static/karta-logo.png" alt="compass shaped logo" height="90" width="100"
	     style="opacity:0.7;filter:alpha(opacity=70);"/>
      </a>
      <h2><a href="/">Karta</a></h2>
      <h3>About</h3>
      Made by <a href="http://elle-est-au-nord.com/" target="_blank">Éléonore</a>
    </div>
    <div class="legend"> Legend </div>
    <div class="map"> Map </div>
  </section>
</template>

<script>

export default {

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

h2 {
  color: #526488;
  padding: 2% 0 30% 0;
}
h2 a {
  text-decoration: none;
  color: #526488;
}
h2 a:hover {
  color: #FFFFFF;
}

h3 {
  color: #526488;
  padding: 20% 0 30% 0;
}

.nav {
  width: 10%;
  min-height: 100vh;
  background-color: rgba(59, 128, 112, 0.7);
}

.legend {
  float: right;
  width: 30%;
  min-height: 100vh;
  background-color: rgba(82, 100, 136, 0.7);
}

.map {
  border: 1px solid green;
  width: 60%;
  min-height: 100vh;
}

</style>
