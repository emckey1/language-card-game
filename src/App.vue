<template>
  <div id="app">
    <div class="mode">
      <ScreenMode />
    </div>
    <Intro title="Welcome to the Language Card Game!!!" subtitle="Click the button below to start the game!!!"/>
    <Button button="Start" />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import Intro from "./components/Intro.vue";
import Button from "./components/Button.vue";
import ScreenMode from './components/ScreenMode.vue';

export default Vue.extend({
  name: "App",
  components: {
    Intro,
    Button,
    ScreenMode
  },
});
</script>

<style scoped class="stylesheet" src='@/assets/style/light.css'></style>