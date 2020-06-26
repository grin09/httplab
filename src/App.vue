<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Nunito:wght@400;600;700&display=swap");
html,
body {
  margin: 0;
  box-sizing: border-box;
  font-family: Nunito, Arial;
  width: 100%;
}
#app {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
</style>
