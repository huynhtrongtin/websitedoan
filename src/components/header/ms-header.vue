<template>
  <div class="ms-header">
    <div class="ms-header-logo">
      <img src="@/assets/logo.png" alt="logo" id="header-logo" />
    </div>
    <div class="ms-header-menu">
      <ul>
        <li><router-link to="/">TRANG CHỦ</router-link></li>
        <li><router-link to="/tuts">VIDEO</router-link></li>
        <li><a href="/book">SÁCH</a></li>
        <li><a href="/blog">BLOG</a></li>
        <li><a href="/question">HỎI ĐÁP</a></li>
      </ul>
      <div class="ms-header-button">
        <a href="/login" target="_blank"
          ><input type="submit" value="Đăng nhập"
        /></a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.ms-header {
  display: flex;
  justify-content: flex-start;
  padding: 0 6vw;

  #header-logo {
    width: 128px;
    height: 90px;
  }

  .ms-header-menu {
    display: flex;
    margin-left: auto;

    ul {
      display: flex;
      align-items: center;

      li {
        list-style-type: none;

        a {
          font-family: serif;
          font-size: 0.857142857142857em;
          text-transform: uppercase;
          font-weight: 600;
          letter-spacing: 0.5px;
          color: #999;
          text-decoration: none;
          margin-right: 2vw;

          &:hover {
            color: #333;
          }
        }
      }
    }

    .ms-header-button {
      display: flex;
      align-items: center;

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

        &:active {
          border: none;
          color: #fff;
        }

        &:hover {
          background-color: #609de6;
          margin-top: -5px;
        }
      }
    }
  }
}
</style>
