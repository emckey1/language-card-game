<template>
  <div class="intro">
    <h1>{{ title }}</h1>
    <h3>{{ subtitle }}</h3>
    <p>
      For this game you will match the French word with the English word.
      Below you can find a list of the English and French Dictionaries.
    </p>
    <ul>
      <li>
        <a href="https://www.dictionary.com/" target="_blank" rel="noopener"
          >English Dictionary</a
        >
      </li>
      <li>
        <a
          href="https://dictionary.cambridge.org/dictionary/french-english/"
          target="_blank"
          rel="noopener"
          >French Dictionary</a
        >
      </li>
    </ul>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: 'Intro',
  props: ['title', 'subtitle']
});
</script>

<style scoped>
  ul {
      list-style-type: none;
      padding: 0;
  }
  
  li {
    margin: 20px;
  }
</style>