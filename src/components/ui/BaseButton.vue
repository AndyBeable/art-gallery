<template>
  <button>
    <span>Our location</span>
    <img src="@/assets/icon-arrow-right.svg" alt="" />
  </button>
</template>

<script>
export default {
  name: "BaseButton",
};
</script>

<style scoped lang="scss">
button {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  border: none;
  padding: 0;
  background-color: var(--black);
  color: var(--white);
  text-transform: uppercase;
  letter-spacing: 3.64px;
  font-weight: 300;
  cursor: pointer;
}

span {
  font-size: 10px;
  margin-left: 10px;
}

img {
  background-color: var(--orange);
  padding: 20px 30px;
}
</style>
