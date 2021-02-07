<template>
    <div class="header-container">
        <div class="header-title">Yoonhye Kim</div>
        <div class="header-sub-container">
            <SbHeaderTitle  content="Home"/>
            <SbHeaderTitle class="m-header-sub-title" content="About"/>
            <SbHeaderTitle class="m-header-sub-title" content="Work"/>
            <sb-button class="m-header-sub-title"/>
        </div>
        
    </div>
</template>

<script>
import SbHeaderTitle from './atoms/SbHeaderTitle.vue'
import SbButton from './atoms/SbButton.vue'

    export default {
        components:{
            SbHeaderTitle,
            SbButton
        }
    }
</script>

<style lang="scss" scoped>

.header-container{
    display: flex;
    background: #121212;
    justify-content: space-between;
    padding: 12px;
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
    align-items: center;
}
.m-header-sub-title{
    margin-left: 20px
}
</style>