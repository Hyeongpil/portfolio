<template>
  <div class="oval-circle" :style="getStyle" />
</template>

<script>
export default {
  props: {
    size: Number,
    background: String
  },
  computed: {
    getStyle() {
      return {
        width: `${this.size}px`,
        height: `${this.size}px`,
        "background-image": this.background
      }
    }
  }
}
</script>

<style lang="scss" scoped>
@keyframes oval-rotate {
  0% {
  }
  100% {
    transform: rotate(360deg);
  }
}

.oval-circle {
  border-radius: 50%;
  opacity: 0.9;
  will-change: transform;
  animation-fill-mode: forwards;
  animation-direction: normal;
  animation-iteration-count: infinite;
  animation-delay: 0s;
  animation-name: oval-rotate;
  animation-duration: 5s;
  animation-timing-function: linear;
}
</style>
