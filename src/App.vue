<script>

import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import FooterApp from './components/FooterApp.vue';
import MerchApp from './components/MerchApp.vue';
import JumbotronApp from './components/JumbotronApp.vue'


export default {
  components:{
    HeaderApp,
    MainApp,
    FooterApp,
    MerchApp,
    JumbotronApp,
  }
};

</script>

<template>

  <HeaderApp/>
  <JumbotronApp/>
  <MainApp/>
  <MerchApp/>
  <FooterApp/>


</template>

<style lang="scss" scoped>
@use './styles/general.scss' as *;
</style>
