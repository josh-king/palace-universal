<template>
  <div class="columns is-centered">
    <div
      v-for="({ name, location }, id) in navigation"
      :key="`palace-nav-${id}`"
      class="column is-3"
    >
      <nuxt-link :to="location" class="has-text-centered">{{ name }}</nuxt-link>
    </div>
  </div>
</template>

<script>
import navigation from '@/assets/data/navigation'

export default {
  data: () => ({
    navigation
  })
}
</script>

<style></style>
