<template>
  <div class="home">
    <Hero />
    <GalleryOverview />
    <Inspiration />
    <Footer />
  </div>
</template>

<script>
import Hero from "../components/home/Hero.vue";
import GalleryOverview from "@/components/home/GalleryOverview";
import Inspiration from "@/components/home/Inspiration";
import Footer from '@/components/ui/Footer'

export default {
  components: {
    Hero,
    GalleryOverview,
    Inspiration,
    Footer
  }
}

</script>
