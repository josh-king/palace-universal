<template>
  <section id="palace-view-init" class="hero is-fullheight">
    <div class="hero-head"></div>
    <div class="hero-body">
      <div class="container">
        <nuxt />
      </div>
    </div>
    <div class="hero-foot">
      <module-footer />
    </div>
  </section>
</template>

<script>
import ModuleFooter from '@/components/navigation/ModuleFooter'

export default {
  components: {
    ModuleFooter
  }
}
</script>

<style></style>
