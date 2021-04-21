<template>
  <section id="as-section-container">
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

    <div v-for="(content, idx) in cardContent" :key="idx">
      <sb-card class="as-card" :title="content.title" :desc="content.desc" />
    </div>
  </section>
</template>

<script>
import SbCard from "./organisms/SbCard.vue"
export default {
  components: { SbCard },
  data() {
    return {
      cardContent: [
        {
          title: "안녕하세요",
          desc: "asdasdasd"
        },
        {
          title: "2222",
          desc: "333"
        },
        {
          title: "444",
          desc: "555"
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
#as-section-container {
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
.as-card {
  margin-bottom: 44px;
}
</style>
