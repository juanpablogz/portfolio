<template>
  <div>
    <script
      src="https://kit.fontawesome.com/da3a675f26.js"
      crossorigin="anonymous"
    ></script>
    <div class="grid-container">
      <div class="social">
        <Social />
      </div>
      <div class="header">
        <Header />
      </div>
      <div class="hero">
        <Hero />
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@900&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Noto+Sans+TC:wght@900&family=Roboto+Mono:ital,wght@1,300&display=swap');
</style>
<style>
body {
  background-color: #13293d;
}
.grid-container {
  display: grid;
  grid-template-columns: 0.3fr 1fr 1fr 1fr;
  grid-template-rows: 0.2fr 1.6fr 1fr;
  gap: 0px 0px;
  grid-template-areas:
    'social header header header'
    'social hero hero hero'
    'social hero hero hero';
}
.social {
  grid-area: social;
}
.header {
  grid-area: header;
}
.hero {
  grid-area: hero;
}
@media screen and (max-width: 768px) {
}
</style>
