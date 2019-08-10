<template>
  <p>{{ this.$route.params.name }}</p>
</template>

<script>
export default {
  layout: 'palace-default',
  mounted() {
    console.log(this.$route.params.name)
  }
}
</script>

<style></style>
