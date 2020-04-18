<template>
  <div :style="classObject" class="hexagon"></div>
</template>

<script>
export default {
  name: 'Hexagon',
  props: {
    height: {
      type: String,
      default: '110px'
    },
    width: {
      type: String,
      default: '100px'
    },
    bgColor: {
      type: String,
      default: '#111'
    }
  },
  computed: {
    classObject: function () {
      return {
        'position': 'relative',
        'height': this.height,
        'width': this.width,
        'background': this.bgColor,
        'margin': '1px',
      }
    }
  }
};
</script>

<style>
.hexagon{
  position: relative;
  margin: 1px;
  clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
  transition: 2s;
}
.hexagon:before{
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 50%;
  height: 100%;
  pointer-events: none;
  background: rgba(255, 255, 255, 0.02);
}
.hexagon:hover{
  transition: 0s;
  background: #0f0;
  cursor: alias;
}
</style>