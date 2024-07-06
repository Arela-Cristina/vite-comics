<script>
import AppHeader from './components/AppHeader.vue'
import AppMainContent from './components/AppMainContent.vue'
import FooterStore from './components/Footer/FooterStore.vue'
import FooterLinks from './components/Footer/FooterLinks.vue'
import FooterSocial from './components/Footer/FooterSocial.vue'

export default {
  components: {
    AppHeader,
    AppMainContent,
    FooterStore,
    FooterLinks,
    FooterSocial
  }
}
</script>

<template>
   <AppHeader />
   <AppMainContent/>
   <FooterStore/>
   <FooterLinks/>
   <FooterSocial/>
    
   
</template>
<!-- hemos quitado scope para importar todos nuestros files -->
<style  lang="scss">
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
