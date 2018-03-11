<template>
  <div class="wrapper">
    <div class="container">
      <nuxt/>
    </div>
    <div class="credits">Icons made by 
      <a href="https://www.flaticon.com/authors/lucy-g" title="Lucy G">Lucy G</a>,
      <a href="https://www.flaticon.com/authors/smashicons" title="Smashicons">Smashicons</a>,
      <a href="https://www.flaticon.com/authors/dave-gandy" title="Dave Gandy">Dave Gandy</a>
      from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a> is licensed by <a href="http://creativecommons.org/licenses/by/3.0/" title="Creative Commons BY 3.0" target="_blank">CC 3.0 BY</a></div>
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

.credits, .credits a {
  font-size: 9px;
  color: #484c4e;
  margin-top: 5px;
}

.icon {
  width: 12px;
  height: 12px;
  vertical-align: middle;
}

@media (max-width: 600px) {
  .wrapper {
    padding: 20px;
  }
  .container {
    padding: 10px;
  }
}
</style>
