<template>
  <div class="fs-section-container">
    <div class="fs-text-container">
      <span class="fs-first-text">Design</span>
      <span class="fs-second-text">Link</span>
      <span class="fs-third-text">Hello, I’m yoonhye. Product designer :)</span>
    </div>
    <div class="fs-img-container">
      <div class="fs-face-img">
        <img src="../assets/img/face.png" />
      </div>
      <div class="fs-oval-img">
        <sb-oval-circle
          :size="446"
          background="linear-gradient(to right, #92fe9d 0%, #00c9ff 100%)"
        />
      </div>
      <div class="fs-rotate-container">
        <sb-oval-circle
          class="fs-rotate-mini"
          :size="122"
          background="linear-gradient(to right, #92fe9d 0%, #00c9ff 100%)"
        />
        <sb-rotate-circle class="fs-rotate-circle" :size="60" />
      </div>
    </div>
  </div>
</template>

<script>
import SbOvalCircle from "./atoms/SbOvalCircle.vue"
import SbRotateCircle from "./atoms/SbRotateCircle.vue"
export default {
  components: { SbRotateCircle, SbOvalCircle }
}
</script>

<style lang="scss" scoped>
.fs-text-container {
  display: flex;
  flex-direction: column;
  text-align: left;
  float: left;
  margin-left: 10%;
}
.fs-first-text {
  font-size: 100px;
  font-weight: 800;
  background: linear-gradient(to right, #00e1d2 3%, #00bf7e 85%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.fs-second-text {
  font-size: 100px;
  font-weight: 800;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.06;
  letter-spacing: normal;
  color: #ffffff;
}
.fs-third-text {
  font-size: 24px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.6;
  letter-spacing: normal;
  color: #ffffff;
  margin-top: 43px;
}
.fs-img-container {
  position: relative;
}
.fs-face-img {
  position: absolute;
  top: 30px;
  left: 60%;
  z-index: 1;
}
.fs-oval-img {
  position: absolute;
  top: -120px;
  left: 70%;
  z-index: -1;
}

.fs-oval-circle {
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
.fs-rotate-container {
  position: relative;
  top: -50px;
  left: -10px;
  z-index: -1;
}
.fs-rotate-mini {
  position: absolute;
  z-index: -1;
}
.fs-rotate-circle {
  position: absolute;
  left: 85px;
  top: -20px;
  z-index: 1;
}
</style>
