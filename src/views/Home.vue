<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <counter/>
    <counterSquared/>
    <buttons/>
    <colorCode/>
  </div>
</template>

<script>
import Counter from '../components/Counter.vue'
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
    'counter': require('@/components/Counter.vue').default,
    'counterSquared': require('@/components/CounterSquared.vue').default,
    'buttons': require('@/components/Buttons.vue').default,
    'colorCode': require('@/components/ColorCode.vue').default
  }
}
</script>

<style >
  div{
    margin-bottom: 10px;
  }
  .counter {
    font-size: 80px;
  }
  .buttons button {
    font-size: 40px;
    width: 100px;
  }
</style>
