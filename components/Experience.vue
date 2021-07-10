<template>
    <div>
<div class="lg:flex">
  <div>
      <div class="">
        <div
          id="experience"
          class="mt-16"
        >
          <div class="flex mt-32">
            <p class="number">02.</p>
            <p class="subtitle pl-2 mt">Experiencia</p>
          </div>
          <h2 class="text">
            <p style="color: white">31Rooms noviembre de 2020 - junio de 2020</p> <br>
            Desarrollador front end con vuejs,
            desarrollo de diversos proyectos con tecnologias como vuejs nuxt y quasar. <br> Proyectos como  <a href="https://estrellarestaurante.com/" style="font-weight: bold; color: white">estrella restaurante </a> que es un listado de productos de un restaurante el cual puedes seleccionar segun preferencia y añadirle variantes, despues tienes las opciones de escoger el medio de pago y para finalizar el software te redirigue a whatsapp con un mensaje personalizado de tu pedido, <a href="https://www.since.love/" style="font-weight: bold; color: white">sincelove</a> que es un proyecto de citas en el cual ayude en el front end realizando diversos componenete en los cuales el más destacado fue la sección de video llamada
          </h2>
        </div>
      </div>
  </div>
  <div>
      <div class="br-2"> 
      <div class=" lg:mt-40 desktop">
          <h2 class="text mt-12">
          <p style="color: white">Especialista en casa Junio de 2018 - Presente (emprendimiento propio)</p> <br>
          <a href="https://www.especialistaencasa.com/" style="font-weight: bold; color: white">Especialista en casa</a> front end de todo el software con el que se controlan servicios médicos, especialmente servicios de fisioterapia. Este servicio puede ser tomado de manera remota y en el domicilio del paciente
          </h2>
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
  color: #FFFCF2;
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
  border-radius: 20px;
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
    // background-color: rgba(100, 255, 218, 0.5);
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

@media (min-width: 600px) {
.desktop {
    margin-top: 11rem;
    padding-left: 75px;
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