<template>
    <div class="header-sub-title">
        {{content}}
    </div>
</template>

<script>
    export default {
        props: {
            content: String
        }
    }
</script>

<style lang="scss" scoped>
.header-sub-title{
  font-size: 16px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
  cursor: pointer;
}
</style>