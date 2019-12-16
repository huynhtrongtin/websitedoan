<template>
  <div class="sign-up-form" v-if="!showSignUp">
    <div class="sign-up-form-container">
      <div class="sign-up-form-container-title">
        <h2>Chọn tư cách đăng nhập</h2>
      </div>
      <div class="sign-up-form-container-content">
        <label for="rdql"
          ><input type="radio" name="gender" value="rdql" id="rdql" />Quản
          lý</label
        >
        <label for="rdkg"
          ><input type="radio" name="gender" value="rdkg" id="rdkg" />Khán
          giả</label
        >
        <div
          class="sign-up-form-container-content-capcha"
          @click="showModal = !showModal"
        >
          <button>
            <img src="capcha-1.png" alt="logocapcha" v-if="!showResultRight" />
          </button>
          <button>
            <img src="capcha-2.png" alt="logocapcha" v-if="showResultRight" />
          </button>
        </div>
        <div class="result-capcha" v-if="showResultRight">
          <h3>Thành công!</h3>
        </div>
        <div class="result-capcha" v-if="showResultWrong">
          <h3>Sai rồi!</h3>
        </div>
      </div>
      <div class="sign-up-form-submit" @click="checkRadio">
        <input type="submit" @click="showSignUp = true" />
      </div>
    </div>
    <div class="modal-capcha" v-if="showModal">
      <img src="sheep.gif" alt="countSheep" />
      <input
        type="text"
        placeholder="Nhập số cừu bạn điếm được"
        id="checksheep"
        ref="checksheep"
      />
      <button @click="checkSheep" v-if="showModal">Check</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showSignUp: false,
      showModal: false,
      showResultRight: false,
      showResultWrong: false,
      showFormQL: false,
      showFormKG: false
    };
  },

  methods: {
    checkSheep: function() {
      const result = document.getElementById("checksheep").value;
      if (result === "12") {
        this.showResultRight = true;
        this.showResultWrong = false;
        this.showModal = false;
      } else {
        this.showResultWrong = true;
        this.showResultRight = false;
        this.showModal = false;
      }
    },

    checkRadio: function() {
      const checkql = document.getElementById("rdql").checked;
      const checkkg = document.getElementById("rdkg").checked;
      if (checkql == true) {
        this.showFormQL = true;
        this.showFormKG = false;
      }
      if (checkkg == true) {
        this.showFormQL = false;
        this.showFormKG = true;
      }
    }
  }
};
</script>

<style lang="scss" scoped>
.sign-up-form {
  top: 0;
  width: 100%;
  height: 100vh;
  position: fixed;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgba(133, 128, 111, 0.5);

  .sign-up-form-container {
    width: 25%;
    position: fixed;
    text-align: center;
    background-color: #fff;
    border-radius: 10px;

    .sign-up-form-container-content {
      label {
        margin-right: 25px;
        margin-left: 25px;
      }
    }

    .sign-up-form-container-content-capcha {
      margin-top: 3vh;

      img {
        width: 23vw;
      }

      button {
        border: none;
        background: transparent;
      }
    }
  }

  .sign-up-form-submit {
    margin-top: 3vh;
    padding-bottom: 20px;
  }

  .modal-capcha {
    width: 25%;
    margin: 30px;
    position: fixed;
    text-align: center;

    img {
      width: 30vw;
      border-radius: 30px;
    }

    input {
      width: 20vw;
      height: 4vh;
    }

    button {
      height: 5vh;
      border: none;
      background-color: #007bff;

      &:hover {
        opacity: 0.6;
      }
    }
  }
}
</style>
