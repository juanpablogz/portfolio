<template>
  <div class="">
    <header class="pr-4 mt-4">
      <div class="lg:hidden">
        <div style="display: flex; justify-content: flex-end">
          <!-- <button
            @click="isOpen = !isOpen"
            class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400"
          >
            <svg
              class="fill-current h-3 w-3"
              viewBox="0 0 20 20"
              xmlns="http://www.w3.org/2000/svg"
            >
              <title>Menu</title>
              <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
            </svg>
          </button> -->
        </div>
      </div>
      <div>
        <ul class="flex header">
          <div class="logo">
            <img
              class="pl-6"
              src="https://res.cloudinary.com/dutj1bbos/image/upload/c_scale,w_80/v1611003309/logo-green_usati5.png"
              alt=""
            />
          </div>
            <div class="flex ">
              <p class="xl:pr-4  color padd">1.</p>
              <a href="https://juanpablogz-d6d32.web.app/" class="letter xl:pr-8 padd" target="_blank">Blog</a>
              <p class="xl:pr-4  color padd">2.</p>
              <a href="https://curriculum-jpgz.netlify.app/" class="letter xl:pr-8 padd" target="_blank">curriculum</a>
              <p class="xl:pr-4  color padd">3.</p>
              <a href="https://wa.link/m14kt0" class="letter xl:pr-8 padd" target="_blank">Hablemos</a>
            </div>
          
        </ul>
      </div>

      <!-- <ul
        class="flex header fixed"
        :class="isOpen ? 'block' : 'hidden'"
        v-gsap.fromTo="[
          { opacity: 0, y: -200 },
          { opacity: 1, y: 0, duration: 2 },
        ]"
      >
        <div>
          <div class="flex">
            <p class="pr-2 color-mobile">1.</p>
            <a href="https://juanpablogz-d6d32.web.app/" class="letter-mobile pr-4" target="_blank">Blog</a>
            <p class="pr-2 color-mobile">2.</p>
            <a href="https://curriculum-jpgz.netlify.app/" class="letter-mobile pr-4" target="_blank">curriculum</a>
            <p class="pr-2 color-mobile">3.</p>
            <a href="https://wa.link/m14kt0" class="letter-mobile pr-4" target="_blank">Hablemos</a>
          </div>
        </div>
      </ul> -->
    </header>
  </div>
</template>

<script>
import { mapGetters } from 'vuex'
export default {
  data() {
    return {
      category: ['Inicio', 'Sobre mi', 'proyectos'],
      isOpen: false,
    }
  },
  created() {
    console.log(this.dataModal)
  },
  computed: {
    dataModal: {
      get() {
        return this.$store.state.albums
      },
    },
  },
  methods: {},
}
</script>
s

<style scoped>
.header {
  justify-content: flex-end;
}
.color {
  color: #07beb8;
}
.letter {
  color: #FFFCF2;
  cursor: pointer;
}
.color-mobile {
  color: #07beb8;
  font-size: 20px;
}
.letter-mobile {
  color: #8892b0;
  cursor: pointer;
  font-size: 20px;
}
.logo {
  flex: auto;
}
.contact {
  color: #64ffda;
  background-color: transparent;
  border: 1px solid #64ffda;
  border-radius: 5px;
  padding: 0.75rem 1rem;
  font-family: var(--font-mono);
  line-height: 1;
  text-decoration: none;
  cursor: pointer;
  transition: var(--transition);
  margin-left: 15px;
  font-size: var(--fz-xs);
}
@media screen and (max-width: 768px) {
  .hidd {
    display: none;
  }
}
@media (max-width: 600px) {
  .logo {
    display: none;
  }
  .padd {
    padding-right: 10px;
  }
}
</style>
