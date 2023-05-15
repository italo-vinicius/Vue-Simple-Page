<template>
  <div>
    <ul>
      <li v-for="(link, index) in links" v-bind:key="index">
        {{ link }} - {{ index }}
      </li>
    </ul>
    <ul>
      <li v-for="(user) in users" :key="user.name">
        {{ user.name }} - {{ user.age }} ({{ user.language }} developer)
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "Users",
  data() {
    return {
      links: ["Linkedin", "GitHub", "Twitter"],
      users: [
        { name: "italo", age: 21, language: "php" },
        { name: "vini", age: 25, language: "js" },
        { name: "gabris", age: 18, language: "pythonzera" },
      ],
    };
  },
};
</script>

<style scoped>
ul {
  color: aliceblue;
}
</style>
