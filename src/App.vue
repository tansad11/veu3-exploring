<template>
  <ScoreCounter name="Bob"/>
  <ScoreCounter name="Carol"/>
</template>

<script>

import ScoreCounter from './components/ScoreCounter';  

export default {
  components : {
    ScoreCounter,
  }
}


</script>

<style>
#app {
  font-family: sans-serif;
  font-size: 3rem;
  text-align: center;
}
</style>
