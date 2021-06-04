<template>
    <div class='button'>
        <button id="startButton" @click="clearScreen()" class="button">{{ button }}</button>
    </div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
    name: 'Button',
    props: ['button'],

    methods: {
        clearScreen() {
            document.getElementById("startButton")?.remove();
        },
    },
});
</script>

<style scopred>
  .button {
    border: none;
    color: white;
    padding: 16px 32px;
    text-align: center;
    text-decoration: none;
    display: inline-block;
    font-size: 18px;
    margin: 4px 2px;
    transition-duration: 0.4s;
    cursor: pointer;
}

#startButton {
    background-color: white;
    color: black;
    border: 3px solid green;
}

#startButton:hover {
    background-color: green;
    color: white;
}
</style>
