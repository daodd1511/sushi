<template>
  <main class="content-container">
    <Popular />
    <Sushi />
    <Statistic />
  </main>
</template>
<script>
import Popular from "./Popular.vue"
import Sushi from "./Sushi.vue"
import Statistic from "./Statistic.vue"
export default {
  components:{
    Popular,
    Sushi,
    Statistic,
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/main.scss";

</style>