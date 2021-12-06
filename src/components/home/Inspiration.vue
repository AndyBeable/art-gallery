<template>
  <div class="inspiration__container">
    <div class="inspiration__large__image">
      <img src="../../assets/mobile/image-grid-2.jpg" alt="">
    </div>
    <div class="inspiration__small__image">
      <img src="../../assets/mobile/image-grid-3.jpg" alt="">
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
.inspiration__container {
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

</style>
