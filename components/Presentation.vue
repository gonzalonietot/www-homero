<template>
<div class="container">
  <img src="~/static/homero.jpg" class="rotate linear infinite" width="150" height="150" />
</div>
</template>

<script>
export default {
  name: 'Presentation',
}
</script>
<style>
.container {
  display: flex;
  width: 100vw;
  height: 100vh;
  justify-content: center;
  align-items: center;
}
.rotate {
  animation: rotation 2s;
}

.linear {
  animation-timing-function: linear;
}

.infinite {
  animation-iteration-count: infinite;
}

@keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}
</style>
