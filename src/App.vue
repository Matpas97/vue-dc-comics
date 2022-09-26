<template>
  <div id="app">
    <MainHeader/>
    <MainComponent/>
    <FooterComponent/>

  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue';
import FooterComponent from './components/FooterComponent.vue';
import MainComponent from './components/MainComponent.vue';



export default {
  name: 'App',
  components: {
    MainHeader,
    MainComponent,
    FooterComponent,
  }
   
   
}
</script>

<style lang="scss">
@import './styles/generic.scss';
@import './styles/variables.scss';
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
 
}
</style>
