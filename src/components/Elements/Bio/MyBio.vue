<template>
  <div>
    <h1>My name is {{ name }}</h1>
    <h2>I'm {{ age }} years old</h2>
    <h2>{{ birthPlace }}</h2>
    <h2>{{ currentlocation }}</h2>
    <hr />
    <!-- <NameComp: name="name"/> <CurrentLocation: {{ currentLocation }}> -->
  </div>
</template>

<script setup>
import { ref } from "vue";
// import NameComp
// import BirthPlaceVue from "./BirthPlace.vue";
// import CurrentLocationVue from "./CurrentLocation.vue";

// import AgeCompVue from "./AgeComp.vue";
// import CurrentLocation from "./CurrentLocation.vue";

const props = defineProps({
  name: {
    type: String,
    required: true,
  },
  age: {
    type: Number,
  },
  birthPlace: {
    type: String,
    default: "world",
  },
  currentlocation: {
    type: String,
  },
});
</script>

<style>
/* #divider {
  @apply m4-border;
} */

div {
  display: flex;
  flex-direction: column;
}
</style>
