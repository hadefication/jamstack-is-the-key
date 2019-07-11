<template>
  <div class="absolute inset-2 shadow-lg">
    <slot />

    <div class="absolute right-1 bottom-1">
      <nuxt-link :to="prev" v-if="prev" class="mr-1">Prev</nuxt-link>
      <nuxt-link :to="next" v-if="next" class="ml-1">Next</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  props: ['prev', 'next']
}
</script>

