<template>
<div>
  <NavBar/>
  <VeloPlan/>
</div>
  </template>
  
  <script>
import NavBar from '~/components/NavBar.vue';
import VeloPlan from '~/components/VeloPlan.vue';
  export default {
    name: "BlogView",
    components: { NavBar, VeloPlan }
}
  </script>
  
  <style scoped>

  </style>
  