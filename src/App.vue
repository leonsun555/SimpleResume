<template>
  <div id="app">
    <Resume />
  </div>
</template>

<script>
import Resume from './components/Resume.vue'

export default {
  name: 'App',
  components: {
    Resume
  }
}
</script>

<style scoped>
#app {
  padding: 50px;
  display: flex;
  justify-content: center;
  background-color: #FFF;
  color: rgba(0,0,0,0.95);
  font-size: 15px;
  line-height: 28px;
  letter-spacing: 1px;
  font-family: "微軟正黑體",sans-serif;
} 
</style>
