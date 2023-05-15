<template>
  <div>
    <p id="paragraph">
      Lorem ipsum dolor sit, amet consectetur adipisicing elit. Repudiandae sint
      quas nulla dolorum cumque. Ut, explicabo minus eligendi nulla, voluptas
      maxime delectus consequatur blanditiis, quia aspernatur fugit nobis dicta
      sit.
    </p>
    <!-- <p id="paragraph" v-if="Lorem">
      Texto do if
    </p>
    <p id="paragraph" v-else>
      Texto do else
    </p> -->
  </div>
</template>

<script>
export default {
  name: "Main",
  data() {
    return { 
      Lorem: true
    }
  }
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
</style>
