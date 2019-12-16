<template>
  <div class="ms-list-lesson">
    <div class="ms-list-lesson-post">
      <h4>#0 - Định hướng học lập trình</h4>
      <span>by CodersX</span>
      <div class="ms-list-lesson-post-image">
        <img src="/0-dinh-huong.png" alt="bai hoc 0" />
      </div>
      <div class="ms-list-lesson-post-description">
        <p>
          Community founder cũng đã từng trải qua quá trình tự học lập trình
          giống như bạn bây giờ. Chuỗi video định hướng giúp định hướng các bạn
          muốn học lập trình mà chưa biết bắt đầu từ đâu. Các video chủ yếu nói
          về cách học hiệu quả, trình tự học.
        </p>
        <button
          @click="showModal = !showModal"
          class="ms-list-lesson-post-link"
        >
          Học miễn phí
        </button>
      </div>
      <div class="modal" v-if="showModal" @click="showModal = flase">
        <iframe
          width="50%"
          height="50%"
          src="https://www.youtube.com/embed/tgbNymZ7vqY"
        ></iframe>
      </div>
    </div>
    <div class="ms-list-lesson-post">
      <h4>#1 - JavaScript từ A-Z 2019</h4>
      <span>by CodersX</span>
      <div class="ms-list-lesson-post-image">
        <img src="1-js.jpg" alt="bai hoc 1" />
      </div>
      <div class="ms-list-lesson-post-description">
        <p>
          Khi bắt đầu học lập trình, bạn nên học một ngôn ngữ lập trình trước để
          học cách tư duy. Thế nên chúng ta sẽ học theo tự JS - HTML - CSS.
          Những web developer cũng nên xem lại để củng cố kiến thức. JavaScript
          là một ngôn ngữ dễ học nhưng khó làm chủ.
        </p>
        <button
          @click="showModal = !showModal"
          class="ms-list-lesson-post-link"
        >
          Học miễn phí
        </button>
      </div>
      <div class="modal" v-if="showModal" @click="showModal = flase">
        <iframe
          width="50%"
          height="50%"
          src="https://www.youtube.com/embed/zIjRONNA_8Y"
        ></iframe>
      </div>
    </div>
    <div class="ms-list-lesson-post">
      <h4>#2 - HTML for dummies</h4>
      <span>by CodersX</span>
      <div class="ms-list-lesson-post-image">
        <img src="/2-html.png" alt="bai hoc 2" />
      </div>
      <div class="ms-list-lesson-post-description">
        <p>
          Community founder cũng đã từng trải qua quá trình tự học lập trình
          giống như bạn bây giờ. Chuỗi video định hướng giúp định hướng các bạn
          muốn học lập trình mà chưa biết bắt đầu từ đâu. Các video chủ yếu nói
          về cách học hiệu quả, trình tự học.
        </p>
        <button
          @click="showModal = !showModal"
          class="ms-list-lesson-post-link"
        >
          Học miễn phí
        </button>
      </div>
      <div class="modal" v-if="showModal" @click="showModal = flase">
        <iframe
          width="50%"
          height="50%"
          src="https://www.youtube.com/embed/pKm3AXC71aQ"
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showModal: false
    };
  }
};
</script>

<style lang="scss" scoped>
.ms-list-lesson {
  width: 100%;
  height: 100vh;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: space-evenly;
  margin-top: 20vh;

  .ms-list-lesson-post {
    width: 25.6vw;

    h4 {
      color: #4a90e2;
      font-size: 1.5em;
      font-weight: 500;
      margin: auto;
      margin-bottom: 10px;
    }

    span {
      color: #666;
    }

    .ms-list-lesson-post-image {
      img {
        height: 30vh;
        border-radius: 6px;
        border: 1px solid #eee;
        margin-top: 1.5vh;
      }
    }

    .ms-list-lesson-post-description {
      color: #808080;
      font-weight: 400;
      font-size: 1.2em;
      line-height: 25px;
      letter-spacing: 0.5px;
    }

    .ms-list-lesson-post-link {
      width: 12vw;
      height: 6vh;
      color: #fff;
      text-decoration: none;
      font-size: 1em;
      background-color: #007bff;
      border: none;
      border-radius: 50px;

      &:hover {
        text-decoration: none;
        background-color: #609de6;
        margin-top: -5px;
      }
    }

    .modal {
      width: 100vw;
      height: 100vh;
      position: fixed;
      top: 0;
      left: 0;
      background-color: rgba(133, 128, 111, 0.5);
      backdrop-filter: blur(10px);
      display: flex;
      justify-content: center;
      align-items: center;

      iframe {
        position: relative;
        border-radius: 5%;
      }

      .button-close {
        position: fixed;

        button {
          width: 3vw;
          height: 4vh;
          border: none;
          margin: 5px;
          position: relative;
          background-color: transparent;

          &:hover {
            background-image: radial-gradient(rgb(160, 1, 1), red);
          }
        }
      }
    }
  }
}
</style>
