<script>
import AppHeader from './components/AppHeader.vue';
import AppHero from './components/AppHero.vue';
import LessonBooking from './components/LessonBooking.vue';
import InfoNumber from './components/InfoNumber.vue';
import SectionCourses from './components/SectionCourses.vue';

export default {
  components: {
    AppHeader,
    AppHero,
    LessonBooking,
    InfoNumber,
    SectionCourses
    
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
<InfoNumber></InfoNumber>
<SectionCourses></SectionCourses>

  </main>
</template>

<style lang="scss">
@use './style/generic';

</style>
