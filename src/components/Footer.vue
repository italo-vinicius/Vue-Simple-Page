<template>
  <div>
    <p id="footer">
      &copy; &amp;  {{ user }} 2023. Todos os direitos reservados.
    </p>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      user: "Itinho",
    };
  },
};
</script>

<style scoped>
#footer {
  background-color: #f2f2f2;
  padding: 20px;
  text-align: center;
}
</style>
