<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppAboutUs from './components/AppAboutUs.vue'

export default {
  components: {
    AppHeader,
    AppContent,
    AppAboutUs,
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
    <AppContent />
  </main>

  <!-- About Us -->
  <section>
    <AppAboutUs />
  </section>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables' as *;
</style>
