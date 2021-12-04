<template>
  <div class="home">
    <Hero />
    <GalleryOverview />
    <Inspiration />
  </div>
</template>

<script>
import Hero from '../components/home/Hero.vue'
import GalleryOverview from "@/components/home/GalleryOverview";
import Inspiration from "@/components/home/Inspiration";

export default {
  components: {
    Hero,
    GalleryOverview,
    Inspiration
  }
}

</script>
