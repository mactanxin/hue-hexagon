<template>
  <div class="hexagon"></div>
</template>

<script>
</script>

<style>
.hexagon{
  position: relative;
  height: 110px;
  width: 100px;
  background: #111;
  margin: 1px;
  clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%);
  transition: 2s;
}
</style>