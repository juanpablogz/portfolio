<template>
  <div class="grid-container fixed">
    <div class="favicon">
      <!-- <img
        class="mt-8 pl-8"
        src="https://res.cloudinary.com/dutj1bbos/image/upload/c_scale,w_80/v1611003309/logo-green_usati5.png"
        alt=""
      /> -->
    </div>
    <div class="social">
      <div class="social-media">
        <a class="fab fa-github fa-2x color mb-4" href="https://github.com/juanpablogz" target="_blank"></a>
        <a class="fab fa-linkedin fa-2x color  mb-4" href="https://www.linkedin.com/in/juan-pablo-b9a50a17b/" target="_blank"></a>
      </div>
    </div>
  </div>
</template>
<script>
export default {}
</script>

<style scoped>
.color {
  color: white;
}
.social-media {
  display: grid;
  padding-left: 35px;
}
.grid-container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  gap: 0px 0px;
  grid-template-areas:
    'favicon favicon favicon favicon'
    'favicon favicon favicon favicon'
    'social social social social';
}
.favicon {
  grid-area: favicon;
  height: 550px;
}
.social {
  grid-area: social;
}
</style>
