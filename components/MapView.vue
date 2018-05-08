<template>
  <div class="map">
    <div id="map-wrap" style="height: 100%">
      <no-ssr>
	<l-map :zoom=13 :center="[47.413220, -1.219482]">
	  <l-tilelayer url="http://{s}.tile.osm.org/{z}/{x}/{y}.png"></l-tilelayer>
	  <l-marker :lat-lng="[47.413220, -1.219482]"></l-marker>
	</l-map>
      </no-ssr>
    </div>
  </div>
</template>

<script>
import { LMap, LTileLayer, LMarker } from 'nuxt-leaflet';

export default {
  name: 'MapView'
}
</script>

<style>
.map {
  width: 60%;
  height: 100vh;
}

.map img {
  height: 100vh;
}
</style>
