<template>
  <div class="hero__container">
    <div class="hero__container--image">

      <picture>
        <source
          media="(min-width: 1200px)"
          srcset="../../assets/desktop/image-hero.jpg"
        />
        <source
          media="(min-width: 768px)"
          srcset="../../assets/tablet/image-hero.jpg"
        />
        <img
          src="../../assets/mobile/image-hero.jpg"
          alt="hero image"
          class="hero-image"
        />
      </picture>
    </div>
    <div class="hero__container--copy">
      <h1>Modern <br>Art Gallery</h1>
      <p>
        The artwork in the collection of the Modern Art Gallery all began from a
        spark of inspiration. Will these pieces inspire you? Vist us and find
        out.
      </p>
      <BaseButton />
    </div>

  </div>
</template>

<script>
import BaseButton from "@/components/ui/BaseButton";

export default {
  name: "Hero",
  components: {
    BaseButton
  }
};
</script>

<style scoped lang="scss">
.hero__container {
  margin-bottom: 6rem;
  &--image {
    margin-bottom: 32px;
  }
  &--copy {
    margin: 0px 16px 20px 16px
  }
  &--copy h1 {
    font-weight: 900;
    font-size: 60px;
    text-transform: uppercase;
    line-height: 55px;
    color: var(--black);
    margin-bottom: 32px;
  }

  &--copy p {
    font-size: 18px;
    line-height: 28px;
    margin-bottom: 32px;
  }
}

@media screen and (min-width: 768px) {
  .hero__container {
    display: flex;
  }
}

</style>
