<template>
  <div class="location__container">
    <div class="location__container__title">
      <h4>Our Location</h4>
    </div>
    <div class="location__container__address">
      <h5>99 King Street</h5>
      <p>Newport</p>
      <p>RI 02840</p>
      <p>United States of America</p>
    </div>
    <div class="location__container__detail">
      <p>
        Our newly opened gallery is located near the Edward King House on 99
        King Street, the Modern Art Gallery is free to all visitors and open
        seven days a week from 8am to 9pm.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Location",
};
</script>

<style scoped lang="scss">
.location__container {
  background-color: var(--black);
  padding: 2rem 2rem;

  &__title {
    font-size: 50px;
    text-transform: uppercase;
    color: var(--white);
  }

  &__address {
    color: var(--white);
  }

}



</style>
