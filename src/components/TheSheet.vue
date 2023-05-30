<template>
  <v-sheet :class="customClass" class="pa-2 ma-2 text-center">
    <div>
      {{content}}
      <span>height: 200px</span>
    </div>
  </v-sheet>
</template>

<script>
export default {
  name: 'TheSheet',
  props: {
    customClass: {
      type: String,
      default: '',
    },
    content: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped lang="scss">
.v-sheet {
  border: 1px solid black;
  position: relative;

  div {
    width: 100%;
    display: grid;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
</style>
