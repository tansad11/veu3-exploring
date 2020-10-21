<template>
     <div>
      <h2>{{props.name}}</h2>
      <p>{{player.score}}</p>
      <button @click="decrease()">Decrease</button>
      <button @click="increase()">Increase</button>
    </div>
</template>

<script>
import { reactive } from 'vue'

export default {
    props: {
        name : String,
    },

    setup(props){

      const increase = () =>{
        player.score += 1;
      }

      const decrease = () =>{
        player.score -= 1;
      }

      const player = reactive({
        score : 0
      })

      return {
        props,
        player,
        increase,
        decrease
      }
    }
}

</script>

<style>

</style>