<template>
  <div class="gallery">
    <div class="gallery__copy">
      <h2>Your day at the gallery</h2>
      <p>
        Wander through our distinct collection and find new insights about our
        artists. Dive in to the details of their creative process.
      </p>
    </div>
    <div class="gallery__image">
      <picture>
        <source
          media="(min-width: 1200px)"
          srcset="../../assets/desktop/image-grid-1.jpg"
        />
        <source
          media="(min-width: 768px)"
          srcset="../../assets/tablet/image-grid-1.jpg"
        />
        <img src="../../assets/mobile/image-grid-1.jpg" alt="">
      </picture>
    </div>
  </div>
</template>

<script>
export default {
  name: "GalleryOverview"
};
</script>

<style scoped lang="scss">
.gallery {
  display: flex;
  flex-direction: column-reverse;
  padding: 0 16px;
  margin-bottom: 120px;

  &__copy h2 {
    max-width: 235px;
    margin-bottom: 21px;
  }
  &__image img{
    width: 100%;
    margin-bottom: 25px;
  }
}

@media screen and (min-width: 768px) {
  .gallery__container {
    flex-direction: row;
    justify-content: center;

    &--copy {
      max-width: 300px;
    }
    &--copy h2{
      max-width: 200px;
    }
  }
}
</style>
