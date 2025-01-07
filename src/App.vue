<script setup>
import { onMounted } from "vue";
import NavBar from "./components/NavBar.vue";
import AboutMe from "./components/AboutMe.vue";
import MyProjects from "./components/MyProjects.vue";
import MyEducation from "./components/MyEducation.vue";

 onMounted(() => {
    setTimeout(() => {
      window.HSStaticMethods.autoInit();
    }, 100)
  });
</script>

<template>
  <NavBar/>
  <AboutMe/>
  <MyProjects/>
  <MyEducation/> 
</template>
