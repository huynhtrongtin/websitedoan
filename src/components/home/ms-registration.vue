<template>
  <div class="ms-registration">
    <div class="ms-registration-free">
      <span>FREE</span>
    </div>
    <div class="ms-registration-content">
      <p>
        <a href="#">Đăng ký</a> để nhận ngay <b>khoá học lập trình 1 năm</b> và
        cơ hội <b>đi làm tại Nhật </b>hoàn toàn <b> MIỄN PHÍ. </b>
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.ms-registration {
  width: 100%;
  display: flex;
  justify-content: center;
  margin: 0;
  padding: 0;

  .ms-registration-free {
    display: flex;
    align-items: center;
    position: initial;
    margin-right: 15px;
    margin-top: 5vh;

    span {
      color: #fff;
      font-weight: bold;
      font-family: monospace;
      background-color: #31639c;
      border-radius: 50px 20px;
      padding: 8px 27px;
    }
  }

  .ms-registration-content {
    position: initial;
    display: flex;
    margin-top: 5vh;

    p {
      font-size: 1em;
      font-family: sans-serif;
      color: #999;
      a {
        font-weight: bold;
        color: #4a90e2;
      }

      b {
        color: #666;
      }
    }
  }
}
</style>
