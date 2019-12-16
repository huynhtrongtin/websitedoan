<template>
  <div class="ms-persistence">
    <div class="ms-persistence-title">
      <h2>Kiên trì sẽ thành công</h2>
    </div>
    <div class="ms-persistence-description">
      <p>
        Đa phần những người không thành công là những người không kiên trì. Việc
        học cũng vậy, không có một lĩnh vực nào bạn có thể học và thành tài
        trong chốc lát. Có thể ví chuyện học hành giống như xây một công trình
        mà không bao giờ kết thúc vậy. Công trình của bạn to lớn, vĩ đại tới mức
        nào là do bạn quyết định, nó tương đương với số giờ mà bạn bỏ ra để học
        và thực hành. Do vậy, hãy kiên trì. Đừng để ngày mai bạn vẫn chỉ như
        ngày hôm nay.
      </p>
    </div>
    <div class="ms-persistence-note">
      <p>
        “If today were the last day of your life, would you want to do what you
        are about to do today?”
      </p>
    </div>
    <div class="ms-persistence-author">
      <p><b>Steve Jobs</b></p>
      <p id="ms-persistence-ceo">CEO — Apple Inc.</p>
    </div>
    <div class="ms-persistence-icon">
      <i class="fab fa-facebook-f"></i>
      <i class="fab fa-youtube"></i>
      <i class="fab fa-instagram"></i>
    </div>
    <div class="ms-persistence-made">
      <p>Made with <span>⌨️</span> and <span>🙌</span></p>
    </div>
    <div class="ms-persistence-copyright">
      <p>© 2019 coders-x.com</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.ms-persistence {
  width: 100%;
  height: 100vh;
  font-family: sans-serif;
  margin: 0;
  margin-top: 15vh;
  padding: 0;
  text-align: center;

  .ms-persistence-title {
    h2 {
      font-size: 2.5em;
      font-weight: 300;
      margin: 0 auto;
    }
  }

  .ms-persistence-description {
    display: flex;
    justify-content: center;

    p {
      width: 61vw;
      color: #808080;
      font-size: 1.5em;
      line-height: 1.68421053em;
    }
  }

  .ms-persistence-note {
    width: 50vw;
    font-size: 1.6em;
    font-weight: 400;
    color: #808080;
    margin: 0 auto;
  }

  .ms-persistence-author {
    #ms-persistence-ceo {
      font-size: 1em;
      line-height: 1.85714286em;
      font-family: sans-serif;
      font-weight: 400;
      color: #666;
    }
  }

  .ms-persistence-icon {
    i {
      margin-right: 1.5vw;
      color: #666;

      &:hover {
        color: #eee;
      }
    }
  }

  .ms-persistence-made {
    span {
      font-size: 2em;
    }
  }

  .ms-persistence-copyright {
    color: #666;
  }
}
</style>
