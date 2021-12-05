<template>
  <div class="inspiration__container">
    <div class="inspiration__container--image">
      <img src="../../assets/mobile/image-grid-2.jpg" alt="" />
    </div>
    <div class="inspiration__container__details">
      <div class="inspiration__container__details--image">
        <img src="../../assets/mobile/image-grid-3.jpg" alt="" />
      </div>
      <div class="inspiration__container__details--copy">
        <h2>Come & be inspired</h2>
        <p>
          We're excited to welcome you to our gallery and see how our
          collections influence you.
        </p>
      </div>
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
  justify-content: center;
  margin-bottom: 120px;

  &--image {
    margin-bottom: 16px;
  }
}

@media screen and (min-width: 768px) {
  .inspiration__container {
    flex-direction: row;
    justify-content: center;
  }
}

.inspiration__container__details {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 16px;

  & h2 {
    font-size: 50px;
    text-transform: uppercase;
    line-height: 45px;
    font-weight: 900;
    margin-bottom: 21px;
    margin: 0px 16px 24px 16px;
    color: var(--white);
  }

  & p {
    margin: 0px 16px 20px 16px;
    color: var(--white);
  }
  &--copy {
    background-color: var(--black);
    margin: 0 16px;
    padding: 48px 24px 28px 24px;
  }
}


</style>
