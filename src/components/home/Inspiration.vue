<template>
  <div class="inspiration">
    <div class="inspiration__large__image">
      <picture>
        <source
          media="(min-width: 1200px)"
          srcset="../../assets/desktop/image-grid-2.jpg"
        />
        <source
          media="(min-width: 768px)"
          srcset="../../assets/tablet/image-grid-2.jpg"
        />
      <img src="../../assets/mobile/image-grid-2.jpg" alt="">
      </picture>
    </div>
    <div class="inspiration__small__image">
      <picture>
        <source
          media="(min-width: 1200px)"
          srcset="../../assets/desktop/image-grid-3.jpg"
        />
        <source
          media="(min-width: 768px)"
          srcset="../../assets/tablet/image-grid-3.jpg"
        />
      <img src="../../assets/mobile/image-grid-3.jpg" alt="">
      </picture>
    </div>
    <div class="inspiration__copy__container">
      <h4>Come & be inspired</h4>
      <p>
        We're excited to welcome you to our gallery and see how our collections
        influence you.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Inspiration",
};
</script>

<style scoped lang="scss">
.inspiration {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 3rem;
  gap: 16px;
}

.inspiration__copy__container {
  width: 345px;
  margin: 0 auto;
  color: var(--white);
  background-color: var(--black);
  padding: 1.5rem 2.2rem;
}

.inspiration__copy__container h4 {
  font-size: 50px;
  text-transform: uppercase;
  margin-bottom: 1.2rem;
}
.inspiration__copy__container p {
  color: var(--white);
}

@media screen and (min-width: 768px) {
  .inspiration__container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    grid-template-areas:
      "inspiration__large__image inspiration__small__image"
      "inspiration__large__image inspiration__copy__container";
  }
}

@media screen and (min-width: 768px) {
  .inspiration__large__image {
    grid-area: inspiration__large__image;
  }
}

@media screen and (min-width: 768px) {
  .inspiration__small__image {
    grid-area: inspiration__small__image;
  }
}

@media screen and (min-width: 768px) {
  .inspiration__copy__container {
    grid-area: inspiration__copy__container;
   margin: 0;
  }
}


</style>
