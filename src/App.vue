<script setup>
// import NavBarVue from "./components/NavBar.vue";
// import FooterComponentVue from "./components/FooterComponent.vue";
// import Iteration2Vue from "./components/Iteration2.vue";
import { ref } from "vue";
import MyBio from "./components/Elements/Bio/MyBio.vue";

const bands = ref([]);
</script>

<template>
  <!-- <NavBar>
    <iteration-2> </iteration-2>
  </NavBar> -->
  <MyBio
    name="Claudia"
    age="25"
    birthplace="Barcelona"
    currentlocation="Sants"
  />
</template>

<style></style>
