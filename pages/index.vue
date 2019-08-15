<template>
  <div class="columns is-centered is-mobile is-multiline">
    <div
      v-for="({ name, location, colour }, id) in navigation"
      :key="`palace-nav-${id}`"
      class="column is-2-desktop is-7-tablet is-10-mobile"
    >
      <palace-navigation :colour="colour" :location="location" />
    </div>
  </div>
</template>

<script>
import navigation from '@/assets/data/navigation'

import PalaceNavigation from '@/components/page/index/PalaceNavigation'

export default {
  components: {
    PalaceNavigation
  },
  data: () => ({
    navigation
  })
}
</script>

<style>
.image svg {
  fill: blue;
}
</style>
