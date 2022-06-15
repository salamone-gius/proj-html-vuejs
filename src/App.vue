<template>
  <div id="app">
    <BaseHeader/>
    <BaseMain/>
    <BaseFooter/>
  </div>
</template>

<script>
import BaseHeader from './components/header/BaseHeader.vue'
import BaseMain from './components/main/BaseMain.vue'
import BaseFooter from './components/footer/BaseFooter.vue'

export default {
  name: 'App',

  components: {
    BaseHeader,
    BaseMain,
    BaseFooter,
  }
}
</script>

<style lang="scss">
@import './assets/style/global.scss';
@import url('https://fonts.googleapis.com/css2?family=Trocchi&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Work+Sans:wght@100;300;400;500;700;900&display=swap');
</style>
