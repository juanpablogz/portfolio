<template>
  <div>
    <div class="flex mt-32 mb-12">
      <p class="number">01.</p>
      <p class="subtitle pl-2 mt">About Me</p>
    </div>
    <div class="container">
        <div class="item level-1 work">
            <img src="https://static.platzi.com/media/public/uploads/landing_1c67bffd-7af0-4bd0-8370-d640b64c7842.jpg"
                alt="">
        </div>

        <div class="item level-1 work">
            <img src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611333027/screenshot-estrellarestaurante-com-1611332998500_nosdgy.png"
                alt="">
        </div>
        <div class="item level-2 work">
            <img src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611334029/screenshot-zealous-mayer-c3bddc-netlify-app-1611334019534_rnakpp.png"
                alt="">
        </div>
        <div class="item level-3 work">
            <img src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611263920/colombia_jkhpsk.png"
                alt="">
        </div>
                <div class="item level-1 work">
            <img src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611334397/screenshot-www-especialistaencasa-com-1611334362535_jr7pl9.png"
                alt="">
        </div>
        <div class="item level-2 work">
            <img src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611334933/screenshot-exchange25-netlify-app-1611334909363_zpav5a.png"
                alt="">
        </div>
        <div class="item level-3 work">
            <img src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611334578/screenshot-juego25-netlify-app-1611334565950_wsuhou.png"
                alt="">
        </div>
        <!-- <div class="item level-2">
            <img src="https://res.cloudinary.com/dutj1bbos/image/upload/v1611334801/screenshot-appgora-8ae35-firebaseapp-com-1611334789111_dku8kb.png"
                alt="">
        </div> -->
        <!-- <div class="item level-3">
            <img src="https://static.platzi.com/media/public/uploads/house_3efda176-6e03-442d-9749-67736a0776d4.jpg"
                alt="">
        </div> -->
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
    .container {
        display: grid;
        grid-template-columns: repeat(auto-fit, 300px);
        grid-gap: 5px;
    }

    .item {
        border-radius: 5px;
        padding: 10px;
    }

    .item img {
        width: 100%;
        height: 100%;
        object-fit: cover;

    }
.item:nth-of-type(1) {
  display: none;
}
    .level-1 {
        grid-row-end: span 3;
    }

    .level-2 {
        grid-row-end: span 2;
    }

    .level-3 {
        grid-row-end: span 1;
    }
@media screen and (max-width: 768px) {
    .container {
        justify-content: center;
    }
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
.work {
  padding: 1px;
  cursor: pointer;
  position: relative; 
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
.work:hover {
        &::before {
    content: "";
    position: absolute;
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    cursor:pointer;
    background-color: rgba(255,255,255,0.1);
  }
}
</style>
