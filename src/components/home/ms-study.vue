<template>
  <div class="ms-study">
    <div class="ms-study-title">
      <h2>Bạn sẽ học được gì?</h2>
    </div>
    <div class="ms-study-description">
      <p>
        Đến với cộng đồng CodersX không những bạn được học về lập trình miễn
        phí, bạn còn có cơ hội thực tập với những dự án thực tế, có cơ hội được
        giới thiệu tới các công ty lớn tại Nhật Bản.
      </p>
    </div>
    <div class="ms-study-container">
      <div class="ms-study-container-line"></div>
      <ul>
        <li>
          <div class="ms-study-container-item">
            <div class="ms-study-container-item-number">
              <p>1</p>
            </div>
            <div class="ms-study-container-item-text">
              <h4>Học lập trình cơ bản</h4>
              <p>
                Bạn sẽ được làm quen với ngôn ngữ lập trình JavaScript, các ngôn
                ngữ khác phục vụ cho lập trình web như HTML, CSS.
              </p>
            </div>
          </div>
        </li>
        <li>
          <div class="ms-study-container-item">
            <div class="ms-study-container-item-number">
              <p>2</p>
            </div>
            <div class="ms-study-container-item-text">
              <h4>Học lập trình nâng cao</h4>
              <p>
                Khoá học này bao gồm JavaScript nâng cao, các framework được sử
                dụng để lập trình cho front-end và back-end
              </p>
            </div>
          </div>
        </li>
        <li>
          <div class="ms-study-container-item">
            <div class="ms-study-container-item-number">
              <p>3</p>
            </div>
            <div class="ms-study-container-item-text">
              <h4>Làm dự án</h4>
              <p>
                Sau khi học xong lập trình nâng cao, bạn sẽ được thực tập với
                một dự án nhỏ quy mô 1 dev, được người có kinh nghiệm hơn review
                code. Sau đó sẽ thực tập với các dự án lớn hơn, sát với công
                việc thực tế hơn và quy mô team lớn hơn.
              </p>
            </div>
          </div>
        </li>
        <li>
          <div class="ms-study-container-item">
            <div class="ms-study-container-item-number">
              <p>4</p>
            </div>
            <div class="ms-study-container-item-text">
              <h4>Học các kỹ năng để đi làm tại Nhật</h4>
              <p>
                Trước khi sang Nhật làm việc, các bạn sẽ được đào tạo các kĩ
                năng cơ bản để có thể thích nghi được với môi trường làm việc
                của một đất nước công nghiệp, những kĩ năng mà bạn thường không
                được học ở trường lớp.
              </p>
            </div>
          </div>
        </li>
      </ul>
    </div>
    <div class="ms-study-container-image">
      <img src="/code-editor.svg" alt="img" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.ms-study {
  width: 100%;
  border-top: 1px solid #ebebeb;
  margin: 0;
  padding: 0;
  right: 0;
  left: 0;
  padding-top: 25vh;
  background-color: #fafafa;
  padding-bottom: 10vh;
  border-bottom: 1px solid #ebebeb;
  padding-right: 8px;

  .ms-study-title {
    display: flex;
    justify-content: center;
    font-family: sans-serif;

    h2 {
      font-size: 2.5em;
      font-weight: 300;
      margin: 0 auto;
    }
  }

  .ms-study-description {
    p {
      width: 61vw;
      line-height: 1.68421053em;
      font-size: 1.5em;
      color: #808080;
      margin: 0 auto;
      margin-top: 5vh;
    }
  }

  .ms-study-container {
    position: relative;
    margin-top: 5vh;
    margin-left: 3vw;
    font-family: sans-serif;

    .ms-study-container-line {
      width: 10vw;
      height: 95vh;
      position: absolute;
      border-right: 1px dashed #ddd;
      margin-left: -5vw;
      margin-top: 12vh;
    }

    h4 {
      font-weight: 300;
      font-size: 1.7em;
    }

    p {
      width: 28vw;
      color: #666666;
      font-size: 1.2em;
    }

    li {
      list-style-type: none;
    }

    .ms-study-container-item {
      display: flex;
    }

    .ms-study-container-item-text {
      margin-left: 50px;
      margin-top: -25px;
    }

    .ms-study-container-item-number {
      p {
        width: 50px;
        height: 50px;
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
        border: 2px solid blue;
        border-radius: 50%;
        background-color: #fff;
      }
    }
  }

  .ms-study-container-image {
    width: 540px;
    height: 609px;
    position: absolute;
    right: 0;
    margin-top: -120vh;
    margin-right: 5vw;

    img {
      border-radius: 10px;
    }
  }
}
</style>
