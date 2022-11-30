<template>
 <CheckupForm /> 
</template>

<script>
import CheckupForm from "./components/checkUpForm.vue"

export default {
  name: 'App',
  components: {
    CheckupForm
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
:root{
background:#eee;
}

</style>
