<template>
  <div id="app">
    <div id="nav">
<!--      <router-link to="/">Home</router-link> |-->
<!--      <router-link to="/about">About</router-link>-->
    </div>
    <router-view />
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Big+Shoulders+Display:wght@100;300;400;500;700;900&family=IBM+Plex+Sans:wght@400;700&family=Kumbh+Sans:wght@400;700&family=Outfit:wght@300&display=swap');

:root {
  --orange: #d5966c;
  --black: #151515;
  --gray: #444444;
  --white: #ffffff;
}

*,
*::before,
*::after {
  box-sizing: border-box;
}

body,
h1,
h2,
h3,
h4,
h5,
p,
{
  font-family: 'Big Shoulders Display', sans-serif;
  margin: 0;
}

h1 {
  font-size: 60px;
  font-weight: 900;
  text-transform: uppercase;
  line-height: 55px;
}
h2 {
  font-size: 50px;
  text-transform: uppercase;
}

p {
  font-weight: 300;
  line-height: 32px;
  font-size: 18px;
  color: var(--gray);
  font-family: 'Outfit', sans-serif;;
}
</style>
