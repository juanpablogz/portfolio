<template>
    <div>
<div class="lg:flex">
  <div>
      <div class="description">
        <div
          id="experience"
          class="mt-16"
          v-gsap.fromTo="[
            { opacity: 0, y: -200 },
            { opacity: 1, y: 0, duration: 2 },
          ]"
        >
          <!-- about -->
          <div class="flex mt-32">
            <p class="number">01.</p>
            <p class="subtitle pl-2 mt">Sobre mi </p>
          </div>
          <h2 class="text">
            Hola mi nombre es juan pablo, soy desarrollador de software, vivo en medellin,colombia.
          </h2>
          <h2 class="text">
            Desarrollo aplicaciones web, principalmente con Vuejs, Quasar y NuxtJs, lo cual me permite realizar
            Ssr, PWA y aplicaciones mobile para android y ios
          </h2>
          <h2 class="text">
            En el backend he realizado Api rest con ruby on rails 
          </h2>
          <h2 class="text">
            Las principales tecnologias que conozco son: 
          </h2>
          <div class="flex">
            <ul class="text-technologies pr-4">
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
              <li> <i class="fas fa-code color pr-2"></i>HTML/css</li>
              <li> <i class="fas fa-code color pr-2"></i>TailwindCss</li>
            </ul>
            <ul class="text-technologies">
              <li> <i class="fas fa-code color pr-2"></i> Vue js, Vuex</li>
              <li> <i class="fas fa-code color pr-2"></i>Nuxt</li>
              <li> <i class="fas fa-code color pr-2"></i>Quasar</li>
            </ul>
          </div>
        </div>
      </div>
  </div>
  <div>
      <div class="pl-12 br-2"> 
      <div class="about-me lg:mt-32">
          <img class="image" src="https://res.cloudinary.com/dutj1bbos/image/upload/c_scale,h_350,w_400/v1610036619/25-04_unchp6.jpg" alt="">
      </div>
      </div>
  </div>
</div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.text {
  color: #8892b0;
  margin: 20px 0px 0px;
  min-width: 500px;
  max-width: 500px;
}
.subtitle {
  color: white;
  margin: 0px;
  font-size: 20px;
  font-weight: bold;
}
.text-technologies {
  color: #8892b0;
  margin: 20px 0px 0px;

}
.color {
    color: #64ffda;
}
.number {
  color: #64ffda;
  font-size: 20px;
}
.about-me {
  cursor: pointer;
  position: relative; 
  height: 350px;
  width: 400px;
  display: flex;
  align-items: center;
  justify-content: center;
  background-size: cover;
  &::before {
    content: "";
    position: absolute;
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    background-color: rgba(100, 255, 218, 0.5);
  }
}
.about-me:hover {
        &::before {
    content: "";
    position: absolute;
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    cursor:pointer;
    background-color: rgba(255,255,255,0.5);
  }
}
@media (max-width: 600px) {
.text {
  min-width: 400px;
  max-width: 400px;
}
}
@media (max-width: 400px) {
.text {
  min-width: 340px;
  max-width: 340px;
}
}
@media (max-width: 320px) {
.text {
  min-width: 300px;
  max-width: 300px;
}
}
</style>