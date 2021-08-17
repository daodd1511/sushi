<template>
  <main class="content-container">
    <Popular />
    <Sushi />
    <Statistic />
    <Sushi />
    <Feedback />
    <Email />
  </main>
</template>
<script>
import Popular from "./Content/Popular.vue"
import Sushi from "./Content/Sushi.vue"
import Statistic from "./Content/Statistic.vue"
import Feedback from './Content/Feedback.vue'
import Email from './Content/Email.vue';
export default {
  components:{
    Popular,
    Sushi,
    Statistic,
    Feedback,
    Email,
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/main.scss";

</style>