<template>
  <div class="">
    <header class="pr-8 mt-8" >
      <ul class="flex header">
        <div v-for="(value, key) in category" v-bind:key="value.id">
          <div class="flex">
            <p class="pr-4 color"> 0{{ key + 1 }}.</p>
            <a :href="`#${value}`" class="letter pr-8">{{ value }}</a>
          </div>
        </div>
            <button class="contact">Resume</button>
      </ul>
    </header>
  </div>
</template>

<script>
import { mapGetters } from "vuex";
export default {
  data() {
    return {
      category: ['about', 'experience', 'work'],
    }
  },
  created() {
      console.log(this.dataModal)
  },
  computed: {
    dataModal: {
      get() {
        return this.$store.state.albums;
      }
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
    color: #07BEB8
}
.letter {
    color: #8892b0;
    cursor: pointer
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

</style>
