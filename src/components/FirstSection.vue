<template>
    <div class="fs-section-container">
        <div class="fs-text-container">
             <span class="fs-first-text">Design</span>
        <span class="fs-second-text">Link</span>
        <span class="fs-third-text">Hello, I’m yoonhye. Product designer :)</span>
        </div>
        <div class="fs-img-container">
            <div class="fs-face-img">
                <img src="../assets/img/face.png"/>
                </div>
            <div class="fs-oval-img">
                <img src="../assets/img/oval.png"/>
                </div>
            


        </div>
   
    </div>
    
</template>

<script>
    export default {

    }
</script>

<style lang="scss" scoped>
.fs-text-container{
    display: flex;
    flex-direction: column;
    text-align: left;
    float:left;
}
.fs-first-text{
    font-size:100px;
    font-weight:800;
    background: linear-gradient(to right, #00e1d2 3%, #00bf7e 85%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}
.fs-second-text{
  font-size: 100px;
  font-weight: 800;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.06;
  letter-spacing: normal;
  color: #ffffff;
}
.fs-third-text{
     font-size: 24px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.6;
  letter-spacing: normal;
  color: #ffffff;
}
.fs-img-container{
    
}
.fs-face-img{
position: relative;
top: 30px; 
left: 70px;
z-index: 1;
}
.fs-oval-img{
position: relative;
top: -400px;
left: 400px;
z-index: -1;    
}
</style>