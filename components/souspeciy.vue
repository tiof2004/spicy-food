<template>
  <div>{{ spi1 }}</div>
</template>
<script>
export default {
  name: 'SouspeciyComponents',
  props: {
    spi1: {
      type: String,
      default: ''
    },
    spi2: {
      type: String,
      default: ''
    },
    spi3: {
      type: String,
      default: ''
    },
    spi4: {
      type: String,
      default: ''
    }
  }
}
</script>
