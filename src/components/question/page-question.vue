<template>
  <div class="question">
    <div class="question-container">
      <div class="question-container-title">
        <h1>Hỏi đáp</h1>
      </div>
      <div class="question-container-content">
        <div class="question-container-content-left">
          <p><b>1</b></p>
          <span>trả lời</span>
        </div>
        <div class="question-container-content-main">
          <h2><a href="#">Mọi người cho em hỏi với ạ</a></h2>
          <div class="question-container-content-main-text">
            <p>
              Code website của em nó không chạy, bị lỗi 404. Mọi người coi giúp
              với ạ
            </p>
            <img src="/error-question.png" alt="" />
          </div>
          <div class="question-container-content-main-reply">
            <span @click="showDropdown = !showDropdown"
              >Trả lời (1)<i class="fa fa-caret-down"></i
            ></span>
            <div
              class="question-container-content-main-reply-dropdown"
              v-if="showDropdown"
            >
              <h3>Hiếu:</h3>
              <p>Google đi...</p>
              <img src="/google.png" alt="" />
              <input type="text" placeholder="Nhập nội dung..." /><button>
                Gửi
              </button>
            </div>
          </div>
          <hr />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showDropdown: false
    };
  }
};
</script>

<style lang="scss" scoped>
.question {
  width: 100%;
  text-align: center;
  font-family: sans-serif;

  .question-container {
    h1 {
      font-family: monospace;
      font-weight: 300;
      font-size: 2.7em;
    }
  }

  .question-container-content {
    display: flex;
    justify-content: flex-start;
    margin-left: 10vw;

    .question-container-content-left {
      width: 5vw;
    }

    .question-container-content-main {
      margin-left: 5vw;
      text-align: left;

      h4 {
        font-weight: 300;
      }

      a {
        text-decoration: none;
        color: #4a90e2;

        &:hover {
          opacity: 0.8;
          text-decoration: underline;
        }
      }

      hr {
        width: 50vw;
      }

      .question-container-content-main-text {
        img {
          width: 38vw;
          height: 50vh;
        }
      }

      .question-container-content-main-reply {
        span {
          font-size: 1.2em;
        }

        .question-container-content-main-reply-dropdown {
          width: 50vw;
          margin-left: 5vw;
          margin-top: 2vh;

          img {
            width: 30vw;
            height: 40vh;
          }

          input {
            width: 79%;
            height: 5vh;
            border-radius: 10px 0 0 10px;
          }

          button {
            height: 6vh;
            border-radius: 0 10px 10px 0;
          }
        }
      }
    }
  }
}
</style>
