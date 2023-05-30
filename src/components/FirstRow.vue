<template>
    <v-row no-gutters>
      <v-col>
        <TheSheet content="1" />
      </v-col>

      <v-col cols="8">
        <TheSheet content="2" />
      </v-col>

      <v-col>
        <TheSheet content="3" />
      </v-col>
    </v-row>
</template>

<script>
import TheSheet from "@/components/TheSheet.vue";

export default {
  name: 'FirstRow',
  components: {TheSheet}
}
</script>

<style lang="scss" scoped>
.v-sheet {
  height: 200px;
}
</style>