<template>
  <section class="hero is-fullheight">
    <div class="hero-body">
      <div class="container">
        <div class="columns is-centered">
          <div
            v-for="({ name, location }, id) in navigation"
            :key="`palace-nav-${id}`"
            class="column is-3"
          >
            <p class="has-text-centered">{{ name }}</p>
          </div>
        </div>
      </div>
    </div>
    <div class="hero-foot">
      <module-footer />
    </div>
  </section>
</template>

<script>
import navigation from '@/assets/data/navigation'

import ModuleFooter from '@/components/navigation/ModuleFooter'

export default {
  components: {
    ModuleFooter
  },
  data: () => ({
    navigation
  })
}
</script>

<style></style>
