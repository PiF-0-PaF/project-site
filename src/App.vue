<template>
<div class="App"><Main_page/></div>
</template>

<script>
import Main_page from '@/components/Main_page'

export default {
  name: 'App',
  components: {
    Main_page,
  }
}
</script>

<style>
body{
    margin: 0;
    padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
