<template>
  <div class="location">
    <Map />
    <Location />
  </div>
</template>

<script>
import Map from "@/components/location/Map";
import Location from "@/components/location/Location"

export default {
  components: {
    Map,
    Location
  },
};
</script>

<style scoped lang="scss"></style>
