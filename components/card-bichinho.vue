<template lang="pug">
  .card-bichinho-wrapper
    img(:src="imageUrl")
    .card-content
      h2.title {{ title }}

    .card-footer
      button.orange Ver mais
</template>

<script>
export default {
  props: {
    imageUrl: {
      type: String,
      required: false,
      default: 'https://post.medicalnewstoday.com/wp-content/uploads/sites/3/2020/02/322868_1100-1100x628.jpg'
    },
    title: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="postcss" scoped>
.card-bichinho-wrapper {
  @apply flex flex-col bg-white shadow-lg rounded-xl transition-all duration-200;

  &:hover {
    @apply shadow-xl;
  }

  img {
    @apply rounded-t-xl object-cover;
  }

  .card-content {
    @apply px-3 pt-2 flex-grow flex flex-col justify-between;

    .title {
      @apply font-semibold uppercase text-gray-900 text-lg;
    }
  }

  .card-footer {
    @apply px-3 pb-3 self-end;
    button {
      @apply h-8 w-24 rounded-full;
    }
  }
}
</style>
