<template>
  <div id="app">
    <WithLoggerButton>Button with logger</WithLoggerButton>
    <br>
    <br>
    <Button>Button</Button>
  </div>
</template>

<script>
import Button from "./components/Button.vue";
import { withLoggerButton } from "./components/WithLoggerButton";
const ButtonWithLogger = withLoggerButton(Button);

export default {
  name: "App",
  components: {
    Button: Button,
    WithLoggerButton: ButtonWithLogger
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
