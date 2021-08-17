<template>
  <main class="content-container">
    <Popular />
    <Sushi />
  </main>
</template>
<script>
import Popular from "./Popular.vue"
import Sushi from "./Sushi.vue"
export default {
  components:{
    Popular,
    Sushi,
  }
}
</script>

<style lang="scss" scoped>
@import "@/assets/main.scss";

</style>