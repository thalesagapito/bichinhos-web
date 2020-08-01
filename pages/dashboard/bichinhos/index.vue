<template lang="pug">
  .bichinhos-page-wrapper
    .filters
    .cards
      card-bichinho.card(title="luke")
</template>

<script>
import CardBichinho from '~/components/card-bichinho'

export default {
  layout: 'dashboard',
  components: {
    CardBichinho
  }
}
</script>

<style lang="postcss" scoped>
.bichinhos-page-wrapper {
  @apply flex flex-col;

  .cards {
    @apply flex flex-wrap;

    .card {
      @apply w-64 h-64 m-2;
    }
  }
}
</style>
