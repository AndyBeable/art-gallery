<template>
  <l-map style="height: 500px" :zoom="zoom" :center="center">
    <l-tile-layer :url="url" :attribution="attribution"></l-tile-layer>
    <l-marker :lat-lng="markerLatLng"></l-marker>
    <l-marker :lat-lng="[41.481310, -71.310410]">
      <l-icon
        :icon-size="dynamicSize"
        :icon-anchor="dynamicAnchor"
        icon-url="../../assets/icon-location.svg"
      />
    </l-marker>
  </l-map>
</template>

<script>
import {LMap, LTileLayer, LMarker} from 'vue2-leaflet';

export default {
  name: "Map",
  components: {
    LMap,
    LTileLayer,
    LMarker
  },
  data () {
    return {
      url: 'https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
      attribution:
        '&copy; <a target="_blank" href="http://osm.org/copyright">OpenStreetMap</a> contributors',
      zoom: 15,
      center: [41.481310, -71.310410],
      markerLatLng: [41.481310, -71.310410]
    };
  }
}
</script>

<style scoped>


</style>
