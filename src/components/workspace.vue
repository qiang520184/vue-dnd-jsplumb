<template>
  <div class="workspace">
    <left class="left" />
    <center class="conter" />
    <right class="right" />
  </div>
</template>

<script>
import center from './center';
import left from './left';
import right from './right';

export default {
  data() {
    return {

    }
  },
  components: { left, center, right }
}
</script>

<style>
.workspace {
  width: 100%;
  height: 100%;
  position: relative;
}
.left {
  position: absolute;
  left: 0;
  top: 0;
  width: 200px;
  height: 100%;
  border: 1px solid red;
}
.conter {
  /* position: absolute; */
}
.right {
  position: absolute;
  right: 0;
  top: 0;
  width: 200px;
  height: 100%;
  border: 1px solid yellow;
}

</style>