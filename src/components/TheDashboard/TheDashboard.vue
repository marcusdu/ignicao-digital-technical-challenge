<template>
  <section class="dashboard">
    <navbar-dashboard />
    <breadcrumbs-dashboard />

    <section class="dashboard__filters-list">
      <filters-dashboard />
      <list-dashboard />
    </section>

    <pagination-dashboard />
  </section>
</template>

<script>
import BreadcrumbsDashboard from './BreadcrumbsDashboard.vue'
import FiltersDashboard from './FiltersDashboard.vue'
import ListDashboard from './ListDashboard.vue'
import NavbarDashboard from './NavbarDashboard.vue'
import PaginationDashboard from './PaginationDashboard.vue'
export default {
  name: 'TheDashboard',
  components: {
    NavbarDashboard,
    BreadcrumbsDashboard,
    FiltersDashboard,
    ListDashboard,
    PaginationDashboard
  }
}
</script>
NavbarDashboard

<style lang="scss" scoped>
.dashboard {
  width: 100%;
  padding: 2% 2%;
  background-color: #f9f9f9;

  &__filters-list {
    display: flex;

    @media screen and (max-width: 1100px) {
      flex-direction: column;
      flex-wrap: wrap;
    }
  }
}
</style>
