<template>
  <div class="footer-blog">
    <div class="footer-blog-icon">
      <i class="fab fa-facebook-f"></i>
      <i class="fab fa-youtube"></i>
      <i class="fab fa-instagram"></i>
    </div>
    <div class="footer-blog-made">
      <p>Made with <span>⌨️</span> and <span>🙌</span></p>
    </div>
    <div class="footer-blog-copyright">
      <p>© 2019 ABC</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.footer-blog {
  width: 100%;
  font-family: sans-serif;
  margin: 0;
  margin-top: 15vh;
  padding: 0;
  text-align: center;

  .footer-blog-title {
    h2 {
      font-size: 2.5em;
      font-weight: 300;
      margin: 0 auto;
    }
  }

  .footer-blog-description {
    display: flex;
    justify-content: center;

    p {
      width: 61vw;
      color: #808080;
      font-size: 1.5em;
      line-height: 1.68421053em;
    }
  }

  .footer-blog-note {
    width: 50vw;
    font-size: 1.6em;
    font-weight: 400;
    color: #808080;
    margin: 0 auto;
  }

  .footer-blog-author {
    #footer-blog-ceo {
      font-size: 1em;
      line-height: 1.85714286em;
      font-family: sans-serif;
      font-weight: 400;
      color: #666;
    }
  }

  .footer-blog-icon {
    i {
      margin-right: 1.5vw;
      color: #666;

      &:hover {
        color: #eee;
      }
    }
  }

  .footer-blog-made {
    span {
      font-size: 2em;
    }
  }

  .footer-blog-copyright {
    color: #666;
  }
}
</style>
