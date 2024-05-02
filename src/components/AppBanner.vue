<script >
export default {
  data () {
    return {
        title: "ciao",
        imageName:"vue.svg",
    }
  },
  methods: {
      getImagePath(imageName) {
        return new URL(`../assets/${imageName}`, import.meta.url).href;
      },
    },

}
</script>

<template>
  <h1>{{title}}</h1>
  <img :src="getImagePath(imageName)" alt="" />

</template>

<style scoped>
h1{
    color: red;
    
}
</style>
