<template>
  <div id="app">
    <h1>{{msg}}</h1>
    <img
      alt="Vue logo"
      src="./assets/logo.png"
    >
    <Button @onClick="sayHello">Click</Button>
    <Spinner></Spinner>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import { Button, Spinner } from "@tableau/tableau-ui";

export default {
  name: "app",
  data() {
    return {
      msg: "Run React in Vue"
    };
  },
  methods: {
    sayHello() {
      console.log("Helllo");
    }
  },
  components: {
    HelloWorld,
    Button,
    Spinner
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
