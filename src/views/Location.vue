<template>
  <div class="location">
    <Map />
    <Location />
    <Footer theme="orange"/>
  </div>
</template>

<script>
import Map from "@/components/location/Map";
import Location from "@/components/location/Location";
import Footer from '@/components/ui/Footer'

export default {
  components: {
    Map,
    Location,
    Footer
  },
};
</script>

<style scoped lang="scss"></style>
