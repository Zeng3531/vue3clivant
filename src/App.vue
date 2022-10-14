<template>
  <div>
    <nav>
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </nav>
    <router-view />
    <h1 class="text">12333444555</h1>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.text {
  font-size: 3rem;
}

nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

@function px2rem($px) {
  $baseFontSize: 50;
  @return $px / $baseFontSize +rem;
}

@media screen and (min-width: 320px) {
  html {
    font-size: 21.3333px;
  }
}

@media screen and (min-width: 375px) {
  html {
    font-size: 25px;
  }
}

@media screen and (min-width: 750px) {

  /* 设计稿是750px */
  html {
    /* 即1rem=50px */
    font-size: 50px;
    /* 750/15=50 */
  }
}

.box {
  width: pxrem(200);
  height: pxrem(200);
}
</style>
