<template>
  <div class="columns is-centered">
    <div class="column is-9">
      <div class="columns is-multiline">
        <div
          v-for="shop in shops"
          :key="`shop-${shop.location}`"
          class="column is-6"
        >
          <nuxt-link
            :to="`shops/${shop.location}`"
            tag="figure"
            class="image is-5by3"
          >
            <img :src="shop.images[0]" alt="" srcset="" />
          </nuxt-link>
          <h3 class="title has-text-centered is-uppercase is-6">
            {{ shop.name }} shop
          </h3>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import shops from '@/assets/data/shops'

export default {
  layout: 'palace-default',
  data: () => ({
    shops
  })
}
</script>

<style scoped>
.image {
  transition: opacity 0.1s ease-in-out;
}

.image:hover {
  opacity: 0.2;
  cursor: pointer;
}
</style>
