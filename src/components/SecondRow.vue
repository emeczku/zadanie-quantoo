<template>
  <v-row no-gutters>
    <v-col  cols="5">
      <TheSheet content="4" />
    </v-col>

    <v-col cols="5">
      <TheSheet content="5" />
    </v-col>

    <v-col>
      <TheSheet content="6" />
    </v-col>
  </v-row>
</template>

<script>
import TheSheet from "@/components/TheSheet.vue";

export default {
  name: 'SecondRow',
  components: {TheSheet}
}
</script>

<style lang="scss" scoped>
.v-sheet {
  height: 200px;
}
</style>