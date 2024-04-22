<script>
import AppHeader from './components/AppHeader.vue';
import AppHero from './components/AppHero.vue';

export default {
  components: {
    AppHeader,
    AppHero
    
  },
  data() {
    return {
      
    };
  },
  methods:{}
}
</script>

<template>
  <AppHeader></AppHeader>

  <main>
<AppHero></AppHero>
  </main>
</template>

<style lang="scss">
@use './style/generic';

</style>
