<template>
  <div class="gallery__container">
    <div class="gallery__container--copy">
      <h2>Your day at the gallery</h2>
      <p>
        Wander through our distinct collection and find new insights about our
        artists. Dive in to the details of their creative process.
      </p>
    </div>
    <div class="gallery__container--image">
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
.gallery__container {
  display: flex;
  align-items: center;
  flex-direction: column-reverse;
  margin-bottom: 32px;

  &--copy {
    margin: 0px 16px 20px 16px
  }
  &--copy h2 {
    font-size: 50px;
    text-transform: uppercase;
    line-height: 45px;
    font-weight: 900;
    margin-bottom: 21px;
    max-width: 235px;
  }
  &--image {
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
