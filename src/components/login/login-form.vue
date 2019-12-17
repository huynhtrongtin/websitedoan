<template>
  <div class="login">
    <div class="login-video">
      <video id="myVideo" autoplay muted>
        <source src="/video-blog.mp4" type="video/mp4" />
      </video>
    </div>
    <div class="login-form">
      <div class="login-form-logo">
        <img src="/img_avatar2.png" alt="logo" id="header-logo"
        />
      </div>
      <div class="login-form-content">
        <span><b>Đăng nhập</b></span>
        <div class="login-form-content-input">
          <input type="text" name="uname" id="uname" placeholder="Nhập Email" />
          <input
            type="password"
            name="pass"
            id="pass"
            placeholder="Nhập Password"
          />
          <div class="login-form-conent-input-remember">
            <label>
              <input
                type="checkbox"
                @click="showIcon = !showIcon"
                style="font-size"
              />
              Bạn có muốn nhớ mật khẩu không?
              <i style="font-size:25px;" v-if="!showIcon">😗</i
              ><i style="font-size:25px;" v-if="showIcon">😄</i>
            </label>
          </div>
        </div>
        <div class="login-form-content-interactive">
          <button @click="closeTab">Đăng nhập</button>
          <a href="#"> Quên mật khẩu </a>
        </div>
        <div class="login-form-content-social">
          <div class="login-form-content-social-slec">
            <a
              ><button class="login-fb">
                <i class="fab fa-facebook-f"></i>
                <p>Đăng nhập với Facebook</p>
              </button></a
            >
          </div>
          <div class="login-form-content-social-slec">
            <a
              ><button class="login-gg">
                <i class="fab fa-google"></i>
                <p>Đăng nhập với Google</p>
              </button></a
            >
          </div>
          <div class="login-form-sign-up">
            <p>
              <a href="#" @click="showFormSignUp = !showFormSignUp">Đăng ký</a>
              nếu như bạn chưa có tài khoản
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="form-modal" v-if="showFormSignUp">
      <button @click="showFormSignUp = false">X</button>
      <sign-up-form v-if="showFormSignUp"></sign-up-form>
    </div>
  </div>
</template>

<script>
import SignUpForm from "@/components/login/sign-up-form.vue";

export default {
  components: {
    SignUpForm
  },

  methods: {
    closeTab: function() {
      close();
    }
  },

  data() {
    return {
      showIcon: false,
      showFormSignUp: false
    };
  }
};
</script>

<style lang="scss" scoped>
.login {
  width: 100%;
  height: 100vh;
  top: 0;
  left: 0;
  right: 0;
  background: #eee;
  color: #666;
  font-family: sans-serif;

  .login-video {
    position: absolute;
    margin-top: -1.5vh;
    padding-bottom: 1.5vh;
    margin-left: -1vw;

    video {
      width: 103%;
    }
  }

  .login-form {
    width: 25%;
    height: 100vh;
    background-color: #fff;
    text-align: center;
    float: right;
    padding-left: 2vw;
    position: relative;
    margin-top: -1.5vh;
    padding-bottom: 1.5vh;
    margin-right: -0.6vw;
  }

  .login-form-logo {
    img {
      width: 20vw;
      height: 30vh;
      border-radius: 50%;
      margin-bottom: 30px;
    }
  }

  .login-form-content {
    text-align: left;

    span {
      font-weight: 300;
    }

    .login-form-content-input {
      input[type="text"],
      input[type="password"] {
        width: 90%;
        height: 5vh;
        margin-top: 20px;
      }

      .login-form-conent-input-remember {
        margin: 20px 0;
      }
    }

    .login-form-content-interactive {
      margin-bottom: 5vh;

      button {
        width: 8vw;
        height: 5vh;
        color: #fff;
        background-color: #007be8;
        border: none;
        border-radius: 5px;
        margin-right: 7vw;

        &:hover {
          opacity: 0.8;
        }
      }

      a {
        color: #007be8;
        text-decoration: none;

        &:hover {
          text-decoration: underline;
        }
      }
    }

    .login-form-content-social {
      .login-form-content-social-slec {
        margin-bottom: 3vh;

        button {
          width: 23.5vw;
          height: 5.5vh;
          border: none;
          border-radius: 5px;

          &:hover {
            opacity: 0.8;
          }
        }

        .login-fb {
          background-color: #3b5998;
        }

        .login-gg {
          background-color: #a32b1c;
        }

        i {
          height: 100%;
          width: 16px;
          float: left;
          margin-left: 10px;
          border-right: 1px solid #333;
          display: flex;
          align-items: center;
          font-size: 20px;
          color: #fff;
          margin-left: 3px;
          padding-right: 10px;
        }

        p {
          float: left;
          font-family: sans-serif;
          font-weight: 300;
          color: #fff;
          font-size: 1.2em;
          margin-top: 1.5vh;
          margin-left: 7px;
        }
      }
    }

    .login-form-sign-up {
      a {
        color: #007be8;
        text-decoration: none;

        &:hover {
          text-decoration: underline;
        }
      }
    }

    .form-modal {
      top: 0;
      width: 100%;
      height: 100vh;
      position: fixed;
      background-color: rgba(133, 128, 111, 0.5);
    }
  }
}
</style>
