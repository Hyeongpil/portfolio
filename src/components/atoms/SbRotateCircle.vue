<template>
  <div class="dashed-circle" :style="getStyle"></div>
</template>

<script>
export default {
  props: {
    size: Number
  },

  computed: {
    getStyle() {
      return {
        width: `${this.size}px`,
        height: `${this.size}px`
      }
    }
  }
}
</script>

<style lang="scss" scoped>
@keyframes strawberry {
  0% {
    transform: rotate(0);
  }
  100% {
    transform: rotate(1turn);
  }
}

.dashed-circle {
  border: 2px dashed hsla(0, 0%, 100%, 0.3);
  -webkit-animation: strawberry 16s cubic-bezier(0, 0.55, 0.45, 1) infinite forwards;
  animation: strawberry 16s cubic-bezier(0, 0.55, 0.45, 1) infinite forwards;
  animation-duration: 16s;
  animation-timing-function: cubic-bezier(0, 0.55, 0.45, 1);
  animation-delay: 0s;
  animation-iteration-count: infinite;
  animation-direction: normal;
  animation-fill-mode: forwards;
  animation-play-state: running;
  animation-name: strawberry;
  border-radius: 50%;
}
</style>
