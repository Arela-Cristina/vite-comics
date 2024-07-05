<script>
import AppHeader from './components/AppHeader.vue'
import AppMainContent from './components/AppMainContent.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppMainContent,
    AppFooter
    
  }
}
</script>

<template>
   <AppHeader />
   <AppMainContent/>
   <AppFooter/>
   
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
