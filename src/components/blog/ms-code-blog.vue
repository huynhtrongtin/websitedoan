<template>
  <div class="ms-code-blog">
    <video id="myVideo" autoplay muted>
      <source src="/stickman.mp4" type="video/mp4" />
    </video>
    <div class="ms-content">
      <h1>CodersX's Blog</h1>
      <h2>Cùng nhau học lập trình miễn phí</h2>
      <input type="button" value="ĐĂNG KÝ HỌC" />
    </div>
    <hr />
  </div>
</template>

<style lang="scss" scoped>
.ms-code-blog {
  height: 100vh;
  font-family: monospace;
  font-weight: 300;
  letter-spacing: 0.05em;
  position: relative;

  .ms-content {
    width: 100%;
    position: absolute;
    top: 0;
    text-align: center;
    margin-top: 15vh;

    h1 {
      color: #4a90e2;
      font-size: 2.542857em;
    }

    h2 {
      font-size: 2.542857em;
      margin: 8vh 0;
    }

    input {
      width: 145px;
      height: 38px;
      color: #fff;
      font-weight: 600;
      font-size: 0.857142857142857em;
      text-transform: uppercase;
      background-color: #007bff;
      border: none;
      border-radius: 7px;

      &:hover {
        background-color: #609de6;
        margin-top: -5px;
      }
    }
  }

  #myVideo {
    width: 100%;
    height: calc(100vh - 90px);
  }

  hr {
    width: 70vw;
    margin-top: 15vh;
  }
}
</style>
