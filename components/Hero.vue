<template>
  <div class="scroll-container">
    <div
      class="mt-8"
      v-gsap.fromTo="[
        { opacity: 0, y: -200 },
        { opacity: 1, y: 0, duration: 2 },
      ]"
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
      <button class="contact">Hablemos</button>
    </div>
    <!-- about -->
    <About />
    <!-- end about -->
    <!-- experience -->
    <Experience />
    <!-- end experience -->
    <!-- work -->
    <div></div>
    <div class="grid-container-hero flex">
      <div class="image-project">
        <h2 class="mt-12">Some Things I’ve Built</h2>
        <div class="hero"></div>
      </div>
      <div class="description-project">
        <p class="number mt-16 pl-32">Featured Project</p>
        <p class="number pl-32">OctoProfile</p>
        <div class="h-screen flex items-center">
          <div class="shadow rounded-md bg-white w-full max-w-lg h-48">
            <div class="flex items-center px-5 py-3">
              <img
                class="w-10 h-10 object-cover rounded-full"
                alt="User avatar"
                src="https://i.pravatar.cc/200?u=007"
              />
              <div class="mx-3">
                <p class="text-gray-600">
                  New Story from <b>Arya Stark</b>,
                  <a class="text-blue-500 hover:text-blue-400 hover:underline"
                    >Read now</a
                  >.
                </p>
              </div>
            </div>

            <hr />

            <div class="px-5 py-3">
              <h3 class="font-bold text-xs">TAGS</h3>
              <!-- This is the tags container -->
              <div class="my-3 flex flex-wrap -m-1">
                <span
                  class="m-1 bg-gray-200 hover:bg-gray-300 rounded-full px-2 font-bold text-sm leading-loose cursor-pointer"
                  >#winter</span
                >
                <span
                  class="m-1 bg-gray-200 hover:bg-gray-300 rounded-full px-2 font-bold text-sm leading-loose cursor-pointer"
                  >#stark</span
                >
                <span
                  class="m-1 bg-gray-200 hover:bg-gray-300 rounded-full px-2 font-bold text-sm leading-loose cursor-pointer"
                  >#gameofthrones</span
                >
                <span
                  class="m-1 bg-gray-200 hover:bg-gray-300 rounded-full px-2 font-bold text-sm leading-loose cursor-pointer"
                  >#battle</span
                >
                <span
                  class="m-1 bg-gray-200 hover:bg-gray-300 rounded-full px-2 font-bold text-sm leading-loose cursor-pointer"
                  >#jhonsnow</span
                >
                <span
                  class="m-1 bg-gray-200 hover:bg-gray-300 rounded-full px-2 font-bold text-sm leading-loose cursor-pointer"
                  >#kinglandings</span
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
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
  color: #8892b0;
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
</style>
