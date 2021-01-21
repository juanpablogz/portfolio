<template>
  <div>
    <div class="flex mt-32">
      <p class="number">01.</p>
      <p class="subtitle pl-2 mt">About Me</p>
    </div>
    <div class="container">
        <div class="item level-1">
            <img src="https://static.platzi.com/media/public/uploads/landing_1c67bffd-7af0-4bd0-8370-d640b64c7842.jpg"
                alt="">
        </div>

        <div class="item level-1">
            <img src="https://static.platzi.com/media/public/uploads/landing_1c67bffd-7af0-4bd0-8370-d640b64c7842.jpg"
                alt="">
        </div>
        <div class="item level-2">
            <img src="https://static.platzi.com/media/public/uploads/tshirt_5c8c539f-1867-4641-9a68-e27486424f76.jpg"
                alt="">
        </div>
        <div class="item level-3">
            <img src="https://static.platzi.com/media/public/uploads/house_3efda176-6e03-442d-9749-67736a0776d4.jpg"
                alt="">
        </div>
                <div class="item level-1">
            <img src="https://static.platzi.com/media/public/uploads/landing_1c67bffd-7af0-4bd0-8370-d640b64c7842.jpg"
                alt="">
        </div>
        <div class="item level-2">
            <img src="https://static.platzi.com/media/public/uploads/tshirt_5c8c539f-1867-4641-9a68-e27486424f76.jpg"
                alt="">
        </div>
        <div class="item level-3">
            <img src="https://static.platzi.com/media/public/uploads/house_3efda176-6e03-442d-9749-67736a0776d4.jpg"
                alt="">
        </div>
                <div class="item level-1">
            <img src="https://static.platzi.com/media/public/uploads/landing_1c67bffd-7af0-4bd0-8370-d640b64c7842.jpg"
                alt="">
        </div>
        <div class="item level-2">
            <img src="https://static.platzi.com/media/public/uploads/tshirt_5c8c539f-1867-4641-9a68-e27486424f76.jpg"
                alt="">
        </div>
        <div class="item level-3">
            <img src="https://static.platzi.com/media/public/uploads/house_3efda176-6e03-442d-9749-67736a0776d4.jpg"
                alt="">
        </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
    .container {
        display: grid;
        grid-template-columns: repeat(auto-fit, 250px);
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
</style>
