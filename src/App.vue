<template>
  <div id="app">
    <app-header/>
    <app-navigation/>
    <app-breadcrumbs/>
    <main class="inner-width">
      <router-view/>
    </main>
    <app-footer/>
  </div>
</template>


<script>
import AppHeader from '@/components/AppHeader.vue';
import AppNavigation from '@/components/AppNavigation.vue';
import AppBreadcrumbs from '@/components/AppBreadcrumbs.vue';
import AppFooter from '@/components/AppFooter.vue';

export default {
  name: 'App',
  components: {
    'app-header': AppHeader,
    'app-navigation': AppNavigation,
    'app-breadcrumbs': AppBreadcrumbs,
    'app-footer': AppFooter,
  }
}
</script>