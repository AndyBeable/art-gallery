<template>
  <div class="hero">
<!--    <div class="hero__black__background"></div>-->
    <div class="hero__image">
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
    <div class="hero__copy">
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
.hero {
  margin-bottom: 6rem;
  &__image .hero-image {
    width: 100%;
    margin-bottom: 1.5rem;
  }

  &__copy {
    padding: 0 16px;
  }
  &__copy h1 {
    margin-bottom: 15px;
    color: var(--black);
  }

  &__copy p {
    margin-bottom: 32px;
  }
}

@media screen and (min-width: 768px) {
  .hero {
    display: flex;
    align-items: center;
    position: relative;

    &__copy {
      margin-right: 1rem;
      position: absolute;
      max-width: 300px;
      right: 5rem;
    }
  }
}

.hero__black__background {
  background-color: var(--black);
  height: 800px;
  width: 540px;
}
</style>
