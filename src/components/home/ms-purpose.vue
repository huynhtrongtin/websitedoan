<template>
  <div class="ms-purpose">
    <div class="ms-purpose-title">
      <h2>Mục đích của mình là gì?</h2>
    </div>
    <div class="ms-purpose-description">
      <p>
        Mình có một mong muốn là giúp những người nghèo ở khắp nơi trên thế
        giới, những người mà không có tiền mua máy tính, được học và làm quen
        với lập trình. Mình muốn định hướng cho các bạn trẻ thích học lập trình
        mà không biết bắt đầu từ đâu. Với tốc độ thay đổi công nghệ nhanh như
        hiện tại, càng nhiều lập trình viên giỏi hì thế giới càng phát triển
        nhanh hơn.
      </p>
    </div>
    <div class="ms-purpose-note">
      <p>“Stay hungry, stay foolish.”</p>
    </div>
    <div class="ms-purpose-author">
      <p><b>Steve Jobs</b></p>
      <p id="ms-purpose-ceo">CEO — Apple Inc.</p>
    </div>
    <div class="ms-purpose-icon">
      <i class="fab fa-facebook-f"></i>
      <i class="fab fa-youtube"></i>
      <i class="fab fa-instagram"></i>
    </div>
    <div class="ms-purpose-made">
      <p>Made with <span>⌨️</span> and <span>🙌</span></p>
    </div>
    <div class="ms-purpose-copyright">
      <p>© 2019 coders-x.com</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.ms-purpose {
  width: 100%;
  height: 100vh;
  font-family: sans-serif;
  margin: 0;
  margin-top: 15vh;
  padding: 0;
  text-align: center;

  .ms-purpose-title {
    h2 {
      font-size: 2.5em;
      font-weight: 300;
      margin: 0 auto;
    }
  }

  .ms-purpose-description {
    display: flex;
    justify-content: center;

    p {
      width: 61vw;
      color: #808080;
      font-size: 1.5em;
      line-height: 1.68421053em;
    }
  }

  .ms-purpose-note {
    font-size: 1.6em;
    font-weight: 400;
    color: #808080;
  }

  .ms-purpose-author {
    #ms-purpose-ceo {
      font-size: 1em;
      line-height: 1.85714286em;
      font-family: sans-serif;
      font-weight: 400;
      color: #666;
    }
  }

  .ms-purpose-icon {
    i {
      margin-right: 1.5vw;
      color: #666;

      &:hover {
        color: #eee;
      }
    }
  }

  .ms-purpose-made {
    span {
      font-size: 2em;
    }
  }

  .ms-purpose-copyright {
    color: #666;
  }
}
</style>
