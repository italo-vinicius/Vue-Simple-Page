<template>
  <div>
    <form action="" @submit="sendForm($event)">
      <input type="text" v-model="name" id="name" />
      <br />
      <input type="email" v-model="email" id="email" />
      <br />
      <input type="submit" value="Enviar" id="button" />
    </form>
  </div>
</template>

<script>
export default {
  name: "form",
  data() {
    return {
      name: "",
      email: "",
    };
  },

  methods: {
    sendForm(event) {
      event.preventDefault();
      const name = this.name;
      const email = this.email;
      console.log(`${name} e ${email}`);
    },
  },
};
</script>

<style scoped>
div {
  margin: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
}
#name,
#email {
  margin-bottom: 10px;
}

#button {
  border-radius: 10px;
  color: aqua;
  background-image: linear-gradient(to left, #020107, #2400a8, #ff9f1c);
}
</style>
