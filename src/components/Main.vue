<template>
  <div>
    <p id="paragraph">
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Repudiandae sint
      quas nulla dolorum cumque. Ut, explicabo minus eligendi nulla, voluptas
      maxime delectus consequatur blanditiis, quia aspernatur fugit nobis dicta
      sit.
    </p>
    <p v-show="showText" id="pTeste">Esse texto veio da Main no App.vue: {{ testVar }}</p>
  </div>
</template>

<script>
export default {
  name: "Main",
  props: {
    testVar: String,
    showText: Boolean,
  },
};
</script>

<style scoped>
#paragraph {
  border: 2px solid rgb(255, 255, 255);
  background-color: rgb(31, 162, 214);
  color: rgb(255, 255, 255);
  text-align: justify;
  padding: 2px;
}
#pTeste {
  border: 2px solid rgb(255, 255, 255);
  background-color: rgb(214, 31, 31);
  color: rgb(255, 255, 255);
  text-align: justify;
  padding: 2px;
}
</style>
