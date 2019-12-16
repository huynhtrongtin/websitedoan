<template>
  <div class="ms-why-study">
    <div class="ms-why-study-title">
      <h2>Tại sao nên học tại CorderX?</h2>
    </div>
    <div class="ms-why-study-description">
      <p>
        CodersX đang xây dựng một cộng đồng lập trình viên lớn nhất Việt Nam,
        nơi mọi người được học lập trình miễn phí, giúp đỡ nhau cả trong quá
        trình học cũng như đi làm.
      </p>
    </div>
    <div class="ms-why-study-content">
      <div class="ms-why-study-content-post">
        <img src="/where-to-start.svg" alt="where to start" />
        <h4>Bắt đầu từ đâu?</h4>
        <p>
          Khó khăn đầu tiên ai cũng gặp phải khi học lập trình: Bắt đầu từ đâu?
          CodersX có 10 khoá học theo trình tự giúp bạn trở thành developer từ
          con số 0.
        </p>
      </div>
      <div class="ms-why-study-content-post">
        <img src="/community-support.svg" alt="where to start" />
        <h4>Hỗ trợ 24/7</h4>
        <p>
          Nhóm chat trên Slack với hàng ngàn thành viên thân thiện giúp đỡ nhau
          giải quyết các bài tập khó gặp phải trong quá trình học.
        </p>
      </div>
      <div class="ms-why-study-content-post">
        <img src="/study-for-work.svg" alt="where to start" />
        <h4>Học để đi làm</h4>
        <p>
          Các khoá học được cập nhật với các kiến thức mới nhất và ngắn nhất
          giúp bạn tự tin xin việc sau khi học xong.
        </p>
      </div>
      <div class="ms-why-study-content-post">
        <img src="/go-to-japan.svg" alt="where to start" />
        <h4>Đi Nhật miễn phí</h4>
        <p>
          Sau khi học xong các khoá học và bổ sung tiếng Nhật, bạn sẽ có cơ hội
          được giới thiệu tới các doanh nghiệp tại Nhật Bản hoàn toàn miễn phí.
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.ms-why-study {
  width: 100%;
  height: 100vh;
  font-family: sans-serif;
  padding: 0;
  margin-top: 25vh;
  margin-bottom: 25vh;
  text-align: center;

  .ms-why-study-title {
    h2 {
      font-size: 2.5em;
      font-weight: 300;
    }
  }

  .ms-why-study-description {
    width: 59vw;
    text-align: left;
    color: #808080;
    font-size: 1.35714286em;
    margin: 0 auto;
    margin-top: 7vh;

    p {
      line-height: 1.68421053em;
    }
  }

  .ms-why-study-content {
    display: flex;
    justify-content: center;

    .ms-why-study-content-post {
      width: 21%;
      margin-top: 5vh;
      margin: 15px;

      img {
        width: 95%;
        margin: 10px;
      }

      h4 {
        font-weight: 300;
        font-size: 20px;
      }

      p {
        color: #666666;
        line-height: 3.8vh;
      }
    }
  }
}
</style>
