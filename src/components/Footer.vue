<template>
  <div>
    <div>
      <button @click="buttonFooter(), secondEvent(txt)">{{ MsgButton }} -  {{ txt }}</button>
    </div>
    <p id="footer" v-show="showFooter">
      &copy; &amp; <span> {{ user }} </span> 2023. Todos os direitos reservados.
      Me encontre no <a v-bind:href="GitHub" target="_blank">GitHub</a>
    </p>
  </div>
  <reusable/>
</template>

<script>
import Reusable from './Reusable.vue';
export default {
  components: { Reusable },
  name: "Footer",
  data() {
    return {
      user: "Itinho",
      showFooter: true,
      MsgButton: "Mostrar Footer",
      showName: false,
      txt: '',
      GitHub: "https://github.com/italo-vinicius",
    };
  },
  methods: {
    buttonFooter() {
      this.showFooter = !this.showFooter;
      if (!this.showFooter) {
        this.MsgButton = "Mostrar footer";
      } else {
        this.MsgButton = "Esconder footer";
      }
    },
    secondEvent() {
        this.txt = 'clicastes???'
    }
  },
};
</script>

<style scoped>
#footer {
  background-color: #f2f2f2;
  padding: 20px;
  text-align: center;
  border: 5px solid rgb(0, 129, 134);
}
</style>
