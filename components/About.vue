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
            <p class="subtitle pl-2 mt">About Me</p>
          </div>
          <h2 class="text">
            Hello! I'm Brittany, a software engineer based in Boston, MA.
          </h2>
          <h2 class="text">
            enjoy creating things that live on the internet, whether that be
            websites, applications, or anything in between. My goal is to always
            build products that provide pixel-perfect, performant experiences.
          </h2>
          <h2 class="text">
            Shortly after graduating from Northeastern University, I joined the
            engineering team at Upstatement where I work on a wide variety of
            interesting and meaningful projects on a daily basis.
          </h2>
          <h2 class="text">
            Here are a few technologies I've been working with recently:
          </h2>
          <div class="flex">
            <ul class="text pr-4">
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
              <li> <i class="fas fa-code color pr-2"></i> JavasScript</li>
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
            </ul>
            <ul class="text">
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
              <li> <i class="fas fa-code color pr-2"></i>JavasScript</li>
            </ul>
          </div>
        </div>
      </div>
  </div>


  <div>
      <div class="image mt-32">
        <img
          class="mt-8 pl-8 op"
          src="https://res.cloudinary.com/dutj1bbos/image/upload/c_scale,w_300/v1594870419/carousel-3_uwrxl2.png"
          alt=""
        />
      </div>
  </div>
</div>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
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
.number {
  color: #64ffda;
  font-size: 20px;
}
</style>