<template>
  <div class="location">
    <div class="location__title">
      <h4>Our Location</h4>
    </div>
    <div class="location__address">
      <h5>99 King Street</h5>
      <p>Newport</p>
      <p>RI 02840</p>
      <p>United States of America</p>
    </div>
    <div class="location__detail">
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
.location {
  background-color: var(--black);
  padding: 2rem 2rem;

  p {
    color: var(--white);
  }

  &__title {
    font-size: 50px;
    color: var(--white);
    text-transform: uppercase;
    margin-bottom: 48px;
  }

  &__address {
    margin-bottom: 2rem;
  }

  &__address h5 {
    color: var(--orange);
    font-size: 32px;
    font-weight: 900;
    text-transform: uppercase;
    margin-bottom: 1rem;
  }
  &__address p {
   line-height: 40px;
  }
}



</style>
