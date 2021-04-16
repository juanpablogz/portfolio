<template>
  <div>
      <p>Juan Pablo Gomez zapata © {{year}}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {

    }
  },
  created() {},
  computed: {
    year () {
        var date = new Date();
        var year = date.getFullYear();
        return year
    }
  },
  methods: {
  },
}
</script>

<style scoped>
p {
    display: flex;
    justify-content: center;
    padding: 20px;
    color: #FFFCF2;
}
</style>