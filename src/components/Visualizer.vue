<template>
  <div class="visualizer">
    <h1>Je suis le visualizer</h1>
    <canvas id="visualizer"></canvas>
  </div>
</template>

<script>

  import audio from '../assets/sounds/Kaaris - Tchoin.mp3';
  import appStore from '../stores/AppStore';

  export default {
    name: 'visualizer',
    data() {
      return {
        state: appStore.state,
        audio: new Audio(audio)
      }
    },
    mounted() {
      console.log("je suis monté");
    },
  }

</script>

<style>

</style>
