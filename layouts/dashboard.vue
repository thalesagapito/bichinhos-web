<template lang="pug">
  .dashboard-wrapper
    nav
      img.logo
      ul.links
        n-link(to="/dashboard/bichinhos") Bichinhos
        n-link(to="/dashboard/padrinhos") Padrinhos
        n-link(to="/dashboard/contas") Contas
    nuxt
</template>

<script>
export default {
  name: ''
}
</script>

<style lang="postcss" scoped>
.dashboard-wrapper {
  @apply bg-indigo-100;

  nav {
    @apply bg-primary-indigo rounded-b-xl h-16 flex justify-between items-center px-3 mx-4;

    .logo {
      @apply h-12;
    }

    .links {
      @apply flex;

      a {
        @apply text-white text-sm mx-1 px-3 py-2 rounded-lg transition-all duration-200 font-semibold;

        &:hover {
          @apply bg-white bg-opacity-20;
        }

        &:active {
          @apply transform scale-95;
        }
      }
    }
  }
}
</style>
