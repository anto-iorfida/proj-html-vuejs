<script>
import AppHeader from './components/AppHeader.vue';
import AppHero from './components/AppHero.vue';
import LessonBooking from './components/LessonBooking.vue';
import InfoNumber from './components/InfoNumber.vue';
import SectionCourses from './components/SectionCourses.vue';
import InfoInstructors from './components/InfoInstructors.vue';
import Testimonials from './components/Testimonials.vue';
import LatersNews from './components/LatersNews.vue';
import Newsletter from './components/Newsletter.vue';
import AppInfoFooter from './components/AppInfoFooter.vue';

export default {
  components: {
    AppHeader,
    AppHero,
    LessonBooking,
    InfoNumber,
    SectionCourses,
    InfoInstructors,
    Testimonials,
    LatersNews,
    Newsletter,
    AppInfoFooter

  },
  data() {
    return {

    };
  },
  methods: {}
}
</script>

<template>
  <AppHeader></AppHeader>

  <main>
    <AppHero></AppHero>
    <LessonBooking></LessonBooking>
    <InfoNumber></InfoNumber>
    <SectionCourses></SectionCourses>
    <InfoInstructors></InfoInstructors>
    <Testimonials></Testimonials>
    <LatersNews></LatersNews>
    <Newsletter></Newsletter>
  </main>

  <footer>
    <AppInfoFooter></AppInfoFooter>
  </footer>
</template>

<style lang="scss">
@use './style/generic';
</style>
