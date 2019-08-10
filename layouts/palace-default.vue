<template>
  <section id="palace-view-default-init" class="hero is-fullheight">
    <div class="hero-head">
      <div class="container">
        <div class="columns">
          <div class="column is-2">
            <figure class="image is-3by1">
              <img
                src="https://www.palaceskateboards.com/wp-content/themes/palaceskateboards/css/images/text-logo.svg"
                alt="Palace logo"
              />
            </figure>
          </div>
        </div>
      </div>
    </div>
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
