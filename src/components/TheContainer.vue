<template>
  <v-container>
    <slot></slot>
  </v-container>
</template>

<script>
export default {
  name: 'TheContainer'
}
</script>

<style lang="scss">
.v-container {
  max-width: 1170px !important;
}
</style>