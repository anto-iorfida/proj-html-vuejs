<script>
import AppHeader from './components/AppHeader.vue';
import AppHero from './components/AppHero.vue';
import LessonBooking from './components/LessonBooking.vue';

export default {
  components: {
    AppHeader,
    AppHero,
    LessonBooking
    
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
<LessonBooking></LessonBooking>
  </main>
</template>

<style lang="scss">
@use './style/generic';

</style>
