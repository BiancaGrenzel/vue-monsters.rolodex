<template>
  <div id="app">
    <h1 class="title"> Monsters Rolodex </h1>
    <router-view />
  </div>
</template>

<style lang="scss">

#app {
  text-align: center;
  font-family: sans-serif;
}

body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', 'Oxygen',
    'Ubuntu', 'Cantarell', 'Fira Sans', 'Droid Sans', 'Helvetica Neue',
    sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: linear-gradient(
    to left,
    rgba(7, 27, 82, 1) 0%,
    rgba(0, 128, 128, 1) 100%
  );
}

.title{
  font-family:'Bigelow Rules';
  font-size: 72px;
  color: #0ccac4;
}


</style>
