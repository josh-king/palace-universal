<template>
  <section>
    <figure class="image is-5by3">
      <img :src="currentShop.images[0]" alt="" />
    </figure>
  </section>
</template>

<script>
import shops from '@/assets/data/shops'

export default {
  layout: 'palace-default',
  validate({ params }) {
    return shops.some((shop) => shop.location === params.name)
  },
  data: () => ({
    currentShop: {}
  }),
  beforeMount() {
    this.currentShop = shops.find(
      (shop) => shop.location === this.$route.params.name
    )
  },
  mounted() {
    console.log(this.$route.params.name)
  }
}
</script>

<style></style>
