<template>
  <div>
    <script
      src="https://kit.fontawesome.com/da3a675f26.js"
      crossorigin="anonymous"
    ></script>
    <div class="grid-container">
      <div class="item">
          <Header />
      </div>
      <div class="item">
          <Social />
      </div>
      <div class="item">
          <Hero />
      </div>
      <div class="item">
        <Gmail/>
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
  overflow-x: none;
}
.grid-container {
  display: grid;
  grid-template-columns: 10% 85% 5%;
  grid-template-rows: 50px 50px;
  height: 100vh;
  grid-gap: 5px;
  justify-content: center;
}
/* .item {
  background: lightblue;
  padding: 10px;
  border: 1px solid red;
} */
.item:nth-of-type(1) {
  grid-column: 1 / span 3;
  grid-row: 1 / span 1;
}

@media screen and (max-width: 768px) {
.grid-container {
  display: grid;
  grid-template-columns: 100%;
  height: 100vh;
  grid-gap: 5px;
}
.item:nth-of-type(2) {
  display: none;
}
.item:nth-of-type(3) {
  margin: 10px;
}
.item:nth-of-type(4) {
  display: none;
}
}

</style>
