<template>
  <div>
    <p>Count={{ counter.count }}</p>
    <v-btn @click="counter.increment()">Increment</v-btn>
  </div>
</template>

<script setup>
import {useCounterStore} from '@/stores/counter'
const counter=useCounterStore()
</script>
<style lang="scss">
@use './settings';
</style>
