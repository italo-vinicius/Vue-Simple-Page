<template>
  <div id="picture">
    <img :src="picture" alt="avatar foda" />
  </div>
  <ChangeImage @change-image="changeImage" />
</template>

<script>
import ChangeImage from "./ChangeImage.vue";
export default {
  name: "Picture",
  components: { ChangeImage },
  data() {
    return {
      picture: "/img/avatar.jpg",
    };
  },
  methods: {
    changeImage() {
      console.log('aaaa')
      this.picture = "/img/avatar2.jpg";
    },
  },
};
</script>

<style scoped>
#picture {
  margin: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}
img {
  height: 180px;
  width: 150px;
  border-radius: 50%;
}
</style>
