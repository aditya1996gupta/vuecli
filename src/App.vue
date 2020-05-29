<template>
  <div id="app">
    <message v-if="showMsg" msg="Vue Lifecycle Hooks"></message>
    <button @click="showMsg = false">Hide</button>
  </div>
</template>
<script>
import Message from "./components/Message.vue";
export default {
  name: "app",
  components: {
    Message
  },
  data() {
    return {
      showMsg: true
    };
  }
};
</script>

<style lang="scss">
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
