<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'

export default {
  components: {
    AppHeader,
    AppContent,
  }
}
</script>

<template>
  <!-- Header -->
  <header class="container">
    <nav>
      <AppHeader />
    </nav>
  </header>

  <!-- Main -->
  <main>

  </main>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables' as *;
</style>
