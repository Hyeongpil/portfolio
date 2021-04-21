<template>
  <footer id="footer-section-container">
    <span class="footer-title-text">Contact</span>
    <div class="footer-img-container">
      <img class="footer-img" src="../assets/img/behance.png" />
      <img class="footer-img" src="../assets/img/insta.png" />
      <img class="footer-img" src="../assets/img/linkedin.png" />
    </div>
    <span class="footer-copyright-text">© Yoonhye Kim. 2021 all rights reserved.</span>
  </footer>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
#footer-section-container {
  background-color: #1a1c1d;
  height: 440px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  margin-top: 50px;
}

.footer-title-text {
  color: #ffffff;
  font-size: 36px;
  font-weight: bold;
  margin-top: 50px;
  margin-bottom: 117px;
}

.footer-img-container {
  display: flex;
  justify-content: space-around;
  width: 180px;
  margin-bottom: 110px;
  align-self: center;
}

.footer-img {
  width: 38px;
  height: 38px;
  cursor: pointer;
}

.footer-copyright-text {
  color: #ffffff;
  font-size: 14px;
}
</style>
