<template>
  <div id="picture">
    <img :src="picture" alt="avatar foda" />
  </div>
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      picture: "/img/avatar.jpg",
    };
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
