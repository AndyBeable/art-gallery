<template>
  <div class="container">
    <div class="hero">
      <div class="hero__black__background"></div>
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
      <div class="hero__copy__container">
        <h1>Modern <br />Art Gallery</h1>
        <p>
          The artwork in the collection of the Modern Art Gallery all began from
          a spark of inspiration. Will these pieces inspire you? Vist us and
          find out.
        </p>
        <BaseButton />
      </div>
    </div>
  </div>
</template>

<script>
import BaseButton from "@/components/ui/BaseButton";

export default {
  name: "Hero",
  components: {
    BaseButton,
  },
};
</script>

<style scoped lang="scss">
.container {
  max-width: 1440px;
  margin: 0 auto;
}

.hero {
  display: flex;
  flex-direction: column;
  position: relative;
  margin-bottom: 4rem;

  &__copy__container {
    padding: 0 16px;
  }

  & img {
    margin-bottom: 1.5rem;
    width: 100vw;
  }
  & h1 {
    margin-bottom: 15px;
    color: var(--black);
  }

  & p {
    margin-bottom: 32px;
  }

  @media screen and (min-width: 768px) {
    flex-direction: row;
    align-items: center;

    &__copy__container {
      right: 5rem;
      position: absolute;
      max-width: 400px;
    }
    & img {
      max-width: 500px;
    }
  }
}

.hero__black__background {
  display: none;
  flex: none;
}
</style>
