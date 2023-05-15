<template>
  <div>
    <button type="submit" @click="clickSubmit">Teste</button>
    <span v-show="active">Ativado!!!</span>
  </div>
</template>

<script>
export default {
  name: "Reusable",
  data() {
    return {
      active: true,
    };
  },
  methods: {
    clickSubmit() {
      this.active = !this.active;
    },
  },
};
</script>

<style scoped>
button {
  margin-top: 5px;
}
span {
  color: brown;
  font-family: Arial, Helvetica, sans-serif;
  margin-left: 15px;
}
</style>
