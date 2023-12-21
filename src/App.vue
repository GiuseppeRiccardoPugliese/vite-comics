<script>
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppAboutUs from './components/AppAboutUs.vue'
import AppInfo from './components/AppInfo.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppContent,
    AppAboutUs,
    AppInfo,
    AppFooter,
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

  <!-- Info -->
  <section>
    <AppInfo />
  </section>

  <!-- Footer -->
  <footer>
    <AppFooter />
  </footer>
</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/variables' as *;
</style>
