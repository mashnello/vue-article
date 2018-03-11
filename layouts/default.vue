<template>
  <div class="wrapper">
    <div class="container">
      <nuxt/>
    </div>
  </div>
</template>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

.wrapper {
  background-color: #f2f4f5;
  padding: 20px 50px;
}

.container {
  background-color: #ffffff;
  box-shadow: 0 0 3px #e8ebec;
  padding: 40px 30px;
  width: 100%;
}
</style>
