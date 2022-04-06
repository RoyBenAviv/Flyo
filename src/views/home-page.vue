<template>
  <home-header />
  <section class="home-page">
    <div class="home-container">
      <main-content />
      <info-list />
      <stay-productive />
      <review-list />
      <get-started />
      <home-footer />
    </div>
  </section>
</template>

<script>
import homeHeader from '../components/home-header.vue'
import mainContent from '../components/main-content.vue'
import infoList from '../components/info-list.vue'
import stayProductive from '../components/stay-productive.vue'
import reviewList from '../components/review-list.vue'
import getStarted from '../components/get-started.vue'
import homeFooter from '../components/home-footer.vue'

export default {
  name: 'home',

  components: {
    homeHeader,
    mainContent,
    infoList,
    stayProductive,
    reviewList,
    getStarted,
    homeFooter
  },
}
</script>
