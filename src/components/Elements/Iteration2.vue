<template>
  <div id="exercise-2-part-1">
    <h1>{{ 2 + 2 }}</h1>
  </div>
  <div id="exercise-2-part-1">
    <h1>simple sum of 2 numbers</h1>

    <input type="text" v-model="num1" />
    <input type="text" v-model="num2" />
  </div>
</template>

<script setup>
import { ref } from "vue";

//ITERATION 2
const num1 = ref("0");
const num2 = ref("0");

const result = computed(()) => {
    return pareInt(num1.value) +pareInt(num2.value)

}
</script>

<style></style>
