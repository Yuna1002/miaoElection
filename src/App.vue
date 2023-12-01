<template>
  <header></header>
  <main>
    <RouterView></RouterView>
  </main>
</template>

<script>
import { RouterView } from 'vue-router'
export default {
  components: {
    RouterView
  }
}
</script>

<style scoped></style>
