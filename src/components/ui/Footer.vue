<template>
  <div class="footer" :class="footerTheme">
    <div class="footer__container">
      <div class="footer__container__title">
        <h4>
          Modern<br />
          Art Gallery
        </h4>
      </div>
      <div class="footer__container__copy">
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
  </div>
</template>

<script>
export default {
  name: "Footer",
  props: {
    theme: {
      type: String,
      required: false
    }
  },
  computed: {
    footerTheme() {
      return {
        [`footer--t-${this.theme}`]: this.theme,
      }
    }
  },
}
</script>

<style scoped lang="scss">
// _vars.scss
//$mobile: 375px;
//$tablet: 768px;
//$desktop: 1440px;

.footer {
  width: 100vw;
  padding: 48px 16px;
  background-color: var(--black);
  color: var(--white);

  p {
    color: inherit;
  }

  &--t-orange {
    background-color: var(--orange);
    color: var(--black);
  }
}

.footer {

  & h4 {
    font-size: 30px;
    margin-bottom: 38px;
    text-transform: uppercase;
  }
  & p {
    margin-bottom: 38px;
  }
}

@media screen and (min-width: 768px) {
  .footer__container {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    gap: 10px;

    &__title {
      width: 125px;
    }

    &__copy {
      max-width: 350px;
    }
  }
}

.footer__social__links {
  display: flex;
  gap: 20px;

  .footer.footer--t-orange & {
    filter: invert(1);
  }
}

@media screen and (min-width: 768px) {
  .footer__social__links {
    height: 20px;
  }
}
</style>
