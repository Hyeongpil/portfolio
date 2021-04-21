<template>
  <section class="card-container">
    <img class="card-img" :src="require(`@/assets/img/${imgName}`)" />
    <div class="card-text-container">
      <span class="card-text-title">{{ title }}</span>
      <span>{{ desc }}</span>
    </div>
  </section>
</template>

<script>
export default {
  props: {
    title: String,
    desc: String,
    imgName: String
  }
}
</script>

<style lang="scss" scoped>
.card-container {
  background-color: #1a1c1d;
  width: 863px;
  height: 163px;
  padding: 24px;
  display: flex;
  align-items: center;
  flex-direction: row;
  border-radius: 20px;
}
.card-img {
  width: 140px;
  height: 140px;
  border-radius: 8px;
  background-color: #4f5359;
}
.card-text-container {
  display: flex;
  flex-direction: column;
  margin-left: 25px;
}
.card-text-title {
  color: #ffffff;
  font-size: 36px;
  font-weight: bold;
  margin-bottom: 25px;
}
.card-text-desc {
  font-size: 24px;
  font-weight: bold;
  color: #4f5359;
  line-height: 1.6;
}
</style>
