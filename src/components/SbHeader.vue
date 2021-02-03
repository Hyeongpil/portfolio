<template>
    <div class="header-container">
        <div class="header-title">Yoonhye Kim</div>
        <div class="header-sub-container">
            <SbHeaderTitle  content="Home"/>
            <SbHeaderTitle class="m-header-sub-title" content="About"/>
            <SbHeaderTitle class="m-header-sub-title" content="Work"/>
        </div>
        
    </div>
</template>

<script>
import SbHeaderTitle from './atoms/SbHeaderTitle.vue'

    export default {
        components:{
            SbHeaderTitle
        }
    }
</script>

<style lang="scss" scoped>

.header-container{
    display: flex;
    background: #121212;
    justify-content: space-between;
}

.header-title{
  font-size: 30px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
}
.header-sub-container{
    display: flex;
}
.m-header-sub-title{
    margin-left: 20px
}
</style>