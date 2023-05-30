<template>
  <v-row no-gutters>
    <v-col class="left-box">
      <v-sheet class="pa-2 ma-2 text-center">
        7
        <div class="custom-div">1</div>
        <div class="custom-div">2</div>
        <div class="custom-div">3</div>
        <div class="custom-div">4</div>
      </v-sheet>
    </v-col>

    <v-col class="right-box">
      <v-sheet class="pa-2 ma-2 text-center">
        8
        <div class="custom-div">1</div>
        <div class="custom-div">2</div>
      </v-sheet>
    </v-col>
  </v-row>
</template>

<script>
export default {
  name: 'ThirdRow'
}
</script>

<style scoped lang="scss">
.v-sheet {
  border: 1px solid black;
  position: relative;
  height: 400px;
  display: grid;
  align-items: center;


  .custom-div {
    position: absolute;
    background-color: orange;
    width: 100px;
    height: 100px;
    display: grid;
    align-items: center;
  }
}

.left-box {
  .custom-div:nth-child(1) {
    position: absolute;
    top: 0;
    left: 0;
  }

  .custom-div:nth-child(2) {
    position: absolute;
    right: 0;
    top: 0;
  }

  .custom-div:nth-child(3) {
    position: absolute;
    left: 0;
    bottom: 0;
    width: 200px;
    height: 200px;
  }

  .custom-div:nth-child(4) {
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    margin: 0 auto;
  }
}

.right-box {
  .custom-div:nth-child(1) {
    width: 100%;
    position: absolute;
    top: 0;
    left: 0;
  }

  .custom-div:nth-child(2) {
    width: 100%;
    position: absolute;
    right: 0;
    bottom: 100px;
  }
}
</style>