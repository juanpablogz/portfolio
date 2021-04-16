<template>
  <div class="scroll-container">
    <div
      class="mt-8"
    >
      <p class="hero-1">Hola, mi nombre es</p>
      <h2 class="big-title">Juan pablo.</h2>
      <h2 class="big-title">Y constuyo cosas para la web.</h2>
      <p class="text">
        Soy programador de software, estudie en el sena (colombia) y en AIEP
        (chile) y me especializo en la creacion de sitios web, aplicaciones y
        todo lo que conlleva, mis tecnologias favoritas son Vuejs y ruby on
        rails.
      </p>
      <button class="contact" >
              <a href="https://wa.link/m14kt0" class="letter" target="_blank">Hablemos</a>
      </button>
    </div>
    <!-- about -->
    <About />
    <!-- end about -->
    <!-- experience -->
    <Experience />
    <!-- end experience -->
    <!-- work -->
    <Work/>
    <Footer/>
  </div>
</template>

<script>
export default {
  data() {
    return {}
  },
  created() {},
  computed: {},
  methods: {},
}
</script>

<style lang="scss" scoped>
::-webkit-scrollbar {
  display: none;
}
.scroll-container {
  overflow-x: hidden;
}
body {
  overflow: hidden;
}
.hero-1 {
  color: #64ffda;
}
.color {
  color: #64ffda;
}
.big-title {
  color: #FFFCF2;
  margin: 0px;
  font-size: clamp(40px, 8vw, 80px);
}
.text {
  color: #8892b0;
  margin: 20px 0px 0px;
  max-width: 500px;
}
.contact {
  color: #64ffda;
  background-color: transparent;
  border: 1px solid #64ffda;
  border-radius: 7px;
  padding: 1.25rem 1.75rem;
  font-size: var(--fz-sm);
  font-family: var(--font-mono);
  line-height: 1;
  text-decoration: none;
  cursor: pointer;
  transition: var(--transition);
  margin-top: 50px;
}
.scroll-container {
  display: block;
  width: 100%;
  height: 100vh;
  overflow-y: scroll;
  scroll-behavior: smooth;
}
.scroll-page {
  height: 100%;
}
.number {
  color: #64ffda;
  font-size: 20px;
}
.subtitle {
  color: white;
  margin: 0px;
  font-size: 20px;
  font-weight: bold;
}

.demo_wrap {
  position: relative;
  overflow: hidden;
  padding: 16px;
  border: 1px dashed green;
}
.demo_wrap h1 {
  padding: 100px;
  position: relative;
  z-index: 2;
}
.demo_wrap img {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: auto;
  opacity: 0.6;
}
*,
*::before,
*::after {
  box-sizing: border-box;
}

html {
  font-size: 100%;
}
body {
  background-color: #000000;
  font-family: Arial, sans-serif;
  color: #ffffff;
  line-height: 1.5;
}

.hero {
  cursor: pointer;
  position: relative;
  height: 300px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-image: url('https://placekitten.com/1200/800');
  background-size: cover;

  &::before {
    content: '';
    position: absolute;
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    background-color: rgba(100, 255, 218, 0.5);
  }
}
.hero:hover {
  &::before {
    content: '';
    position: absolute;
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    cursor: pointer;
    background-color: rgba(255, 255, 255, 0.5);
  }
}
h1 {
  position: relative;
  color: #ffffff;
  font-size: 14rem;
  line-height: 0.9;
  text-align: center;
}

.grid-container-hero {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr 1fr;
  gap: 0px 0px;
  grid-template-areas:
    'image-project image-project description-project description-project'
    'image-project image-project description-project description-project'
    'image-project image-project description-project description-project';
}
.image-project {
  grid-area: image-project;
}
.description-project {
  grid-area: description-project;
}
@media (max-width: 600px) {
.scroll-container {
  padding: 20px;
}
}
</style>
