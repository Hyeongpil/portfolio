<template>
  <div>
    <div class="as-text-container">
      <div class="as-title-container">
        <span class="as-title-text">About</span>
      </div>

      <div class="as-content-container">
        <div class="as-first-container">
          <div>connect users</div>
          <div>and services</div>
        </div>

        <div class="as-second-container">
          <div>People and people</div>
          <div class="mt-10">People and services</div>
          <div class="mt-10">Furthermore, people and society,</div>
          <div class="mt-10">We pursue a design that becomes a link</div>
          <div class="mt-10">that brings the space closer together.</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.as-text-container {
  display: flex;
  flex-direction: column;
  text-align: left;
  justify-content: center;
}
.as-content-container {
  display: flex;
  flex-direction: row;
  align-items: center;
  margin-top: 50px;
}
.as-title-text {
  background: linear-gradient(to right, #00e1d2 3%, #00bf7e 85%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 36px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: left;
  color: #ffffff;
}
.as-first-container {
  display: flex;
  flex-direction: column;
}
.as-title-container {
  position: relative;
}
.as-first-container div {
  font-size: 80px;
  font-weight: 800;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.25;
  letter-spacing: normal;
  color: #ffffff;
}
.as-second-container {
  display: flex;
  flex-direction: column;
  margin-left: 150px;
}
.as-second-container div {
  float: right;
  font-size: 24px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.25;
  letter-spacing: normal;
  text-align: left;
  color: #ffffff;
}
</style>
