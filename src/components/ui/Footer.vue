<template>
  <div class="footer__container">
    <div class="footer__container--title">
      <h4>
        Modern<br />
        Art Gallery
      </h4>
    </div>
    <div class="footer__container--copy">
      <p>
        The Modern Art Gallery is free to all visitors and open seven days a
        week from 8am to 9pm. Find us at 99 King Street, Newport, USA.
      </p>
    </div>

    <div class="footer__social__links">
      <img src="../../assets/icon-facebook.svg" alt="" />
      <img src="../../assets/icon-instagram.svg" alt="" />
      <img src="../../assets/icon-twitter.svg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped lang="scss">
.footer__container {
  display: flex;
  flex-direction: column;
  background-color: var(--black);
  color: var(--white);
  padding: 48px 16px;

  & h4 {
    font-size: 30px;
    margin-bottom: 38px;
    text-transform: uppercase;
  }
  & p {
    color: var(--white);
    margin-bottom: 38px;
  }
}

@media screen and (min-width: 768px) {
  .footer__container {
    flex-direction: row;
    justify-content: space-between;
    gap: 10px;

    &--title {
      width: 125px;
    }

    &--copy {
      max-width: 350px;
    }
  }
}

.footer__social__links {
  display: flex;
  gap: 20px;
}

@media screen and (min-width: 768px) {
  .footer__social__links {
    height: 20px;
  }
}
</style>
