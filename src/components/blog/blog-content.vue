<template>
  <div class="blog-content">
    <div class="blog-content-post">
      <div class="blog-content-post-title">
        <h2><a href="">Tại sao nên học lập trình.</a></h2>
        <span> Đăng bởi: <b style="color:#333;">Tui</b></span>
      </div>
      <div class="blog-content-post-content">
        <div class="blog-content-post-content-image">
          <img src="/learning-web-development.jpg" alt="post1" />
        </div>
        <div class="blog-content-post-content-text">
          <h4>Lập trình là gì?</h4>
          <p>
            Để làm nghề lập trình, trước hết các bạn phải hiểu thế nào là lập
            trình viên. Lập trình viên là người thiết kế, xây dựng và bảo trì
            các chương trình máy tính (phần mềm). Bằng cách thao tác các đoạn mã
            (các ngôn ngữ) trên các công cụ lập trình, họ có thể tạo ra các
            chương trình mới, sửa lỗi hay nâng cấp chương trình đó để tăng tính
            hiệu quả của việc...
          </p>
          <button @click="showModalPost = !showModalPost">
            <p style="color: #2275d7;">Đọc tiếp>></p>
          </button>
        </div>
      </div>

      <div
        class="modal-post"
        v-if="showModalPost"
        @click="showModalPost = false"
      ></div>
      <div class="modal-post-display" v-if="showModalPost">
        <div class="modal-post-display-content">
          <h4>1. Lập trình là gì?</h4>
          <p>
            Để làm nghề lập trình, trước hết các bạn phải hiểu thế nào là lập
            trình viên. Lập trình viên là người thiết kế, xây dựng và bảo trì
            các chương trình máy tính (phần mềm). Bằng cách thao tác các đoạn mã
            (các ngôn ngữ) trên các công cụ lập trình, họ có thể tạo ra các
            chương trình mới, sửa lỗi hay nâng cấp chương trình đó để tăng tính
            hiệu quả của việc...
          </p>
          <h4>2. Những yếu tố để trở thành Lập trình viên?</h4>
          <p>
            Nghề lập trình đòi hỏi sự sáng tạo cũng như các kỹ năng đánh giá,
            phân tích yêu cầu của dự án, đưa ra các giải pháp thiết kế hoặc cách
            tiếp cận công nghệ mới khi gặp những framework thiết kế chưa kỹ hoặc
            công nghệ thay đổi.
          </p>
          <h4>3. Suy nghĩ một cách logic</h4>
          <p>
            Logic là điều quan trọng nhất trong lập trình. Bạn phải có đủ nhạy
            bén, linh hoạt và khả năng phán xét cao để giải quyết một vấn đề
            triệt để bằng phương pháp logic. Vì thế, nếu không có khả năng suy
            luận logic thì chắc chắn một điều nghề lập trình không thích hợp với
            bạn. Bạn sẽ cảm thấy nhàm chán và nhức đầu khi theo đuổi các đoạn
            code của chương trình, các vấn đề về debug (gỡ rối), về lỗi, về dấu
            chấm, dấu phẩy…
          </p>
          <div class="modal-post-image">
            <img src="learn-to-code.jpg" alt="anh1" />
          </div>
          <h4>4. Tiếp cận vấn đề có thứ tự và luôn chú ý tới chi tiết</h4>
          <p>
            Các lập trình viên nên tập cho mình thói quen cẩn thận và luôn chú ý
            đến từng chi tiết. Đôi khi những chi tiết rất nhỏ, bạn vô tình bỏ
            qua, thì bạn phải ân hận khi mất hàng ngàn giờ chỉ để tìm những lỗi
            nhỏ đó. Bạn cần có kỹ năng truyền đạt thông tin tốt cũng như viết
            chương trình của mình một cách mạch lạc, có cấu trúc để đồng nghiệp
            của bạn có thể biết được tại sao bạn lại viết đoạn mã như vậy và cái
            gì tiếp theo sẽ xảy ra trong chương trình của bạn.
          </p>
        </div>
      </div>
    </div>
    <hr />
    <div class="blog-content-post">
      <div class="blog-content-post-title">
        <h2><a href="">Tại sao nên học JavaScript.</a></h2>
        <span> Đăng bởi: <b style="color:#333;">Tui</b></span>
      </div>
      <div class="blog-content-post-content">
        <div class="blog-content-post-content-image">
          <img src="/Fundamentals-of-JavaScript-Part-2.png" alt="post2" />
        </div>
        <div class="blog-content-post-content-text">
          <h4>JavaScript là gì?</h4>
          <p>
            JavaScript hoặc JS sẽ giúp tăng tính tương tác trên website. Script
            này chạy trên các trình duyệt của người dùng thay vì trên server và
            thường sử dụng thư vuiên của bên thứ 3 nên có thể tăng thêm chức
            năng cho website mà không phải code từ đầu...
          </p>
          <button @click="showModalPost = !showModalPost">
            <p style="color: #2275d7;">Đọc tiếp>></p>
          </button>
        </div>
      </div>

      <div
        class="modal-post"
        v-if="showModalPost"
        @click="showModalPost = false"
      ></div>
      <div class="modal-post-display" v-if="showModalPost">
        <div class="modal-post-display-content">
          <h4>1. JavaScript là gì?</h4>
          <p>
            JavaScript hoặc JS sẽ giúp tăng tính tương tác trên website. Script
            này chạy trên các trình duyệt của người dùng thay vì trên server và
            thường sử dụng thư vuiên của bên thứ 3 nên có thể tăng thêm chức
            năng cho website mà không phải code từ đầu.
          </p>
          <h4>2. Khuyết điểm của JavaScript là gì?</h4>
          <p>
            Mọi ngôn ngữ lập trình đều có các khuyết điểm. Một phần là vì ngôn
            ngữ đó khi phát triển đến một mức độ như JavaScript, nó cũng sẽ thu
            hút lượng lớn hacker, scammer, và những người có ác tâm luôn tìm
            kiếm những lỗ hổng và các lỗi bảo mật để lợi dụng nó. Một số khuyết
            điểm có thể kể đến là
          </p>
          <div>
            <ul>
              <li>Dễ bị khai thác</li>
              <li>
                Có thể được dùng để thực thi mã độc trên máy tính của người dùng
              </li>
              <li>Nhiều khi không được hỗ trợ trên mọi trình duyệt</li>
              <li>JS code snippets lớn</li>
              <li>
                Có thể bị triển khai khác nhau tùy từng thiết bị dẫn đến việc
                không đồng nhất
              </li>
            </ul>
          </div>
          <h4>3. Cách hoạt động của JavaScript trên trang web là gì?</h4>
          <p>
            JavaScript thường được nhúng trực tiếp vào một trang web hoặc được
            tham chiếu qua file .js riêng. Nó là ngôn ngữ phía client, tức là
            script được tải về máy của khách truy cập và được xử lý tại đó thay
            vì phía server là xử lý trên server rồi mới đưa kết quả tới khách
            truy cập.
          </p>
          <p>
            Hãy lưu ý là các trình duyệt web phổ biến cũng hỗ trợ việc người
            dùng có muốn tắt JavaScript hay không. Đó là lý do bạn nên biết
            trang web sẽ hoạt động như thế nào torng trường hợp không có
            JavaScript.
          </p>
          <h4>3. Làm thế nào để thêm JavaScript trên website của bạn?</h4>
          <p>
            Để thêm chuỗi code JavaScript code vào trang web, bạn sẽ cần gắn tag
            script. Ví dụ như sau:
          </p>
          <div class="modal-post-image">
            <img src="learn-to-code.jpg" alt="anh1" />
          </div>
          <h4>4. Tiếp cận vấn đề có thứ tự và luôn chú ý tới chi tiết</h4>
          <p>
            Các lập trình viên nên tập cho mình thói quen cẩn thận và luôn chú ý
            đến từng chi tiết. Đôi khi những chi tiết rất nhỏ, bạn vô tình bỏ
            qua, thì bạn phải ân hận khi mất hàng ngàn giờ chỉ để tìm những lỗi
            nhỏ đó. Bạn cần có kỹ năng truyền đạt thông tin tốt cũng như viết
            chương trình của mình một cách mạch lạc, có cấu trúc để đồng nghiệp
            của bạn có thể biết được tại sao bạn lại viết đoạn mã như vậy và cái
            gì tiếp theo sẽ xảy ra trong chương trình của bạn.
          </p>
        </div>
      </div>
    </div>
    <hr />
    <div class="footer">
      <footer-blog></footer-blog>
    </div>
  </div>
</template>

<script>
import FooterBlog from "@/components/blog/footer-blog.vue";

export default {
  data() {
    return {
      showModalPost: false
    };
  },

  components: {
    FooterBlog
  }
};
</script>

<style lang="scss" scoped>
.blog-content {
  margin-top: 30vh;
  font-family: sans-serif;

  a {
    text-decoration: none;
  }

  hr {
    width: 60vw;
    margin: 60px auto;
  }

  .blog-content-post {
    text-align: center;
    font-family: sans-serif;
    font-size: 1.3em;
    position: relative;

    .blog-content-post-title {
      h2 {
        font-size: 2.5em;
        font-weight: 300;
        font-weight: bold;
        margin-bottom: 15px;

        a {
          color: #333;
          &:hover {
            color: #999;
          }
        }
      }

      span {
        color: #999;
        font-weight: 300;
        font-size: 1em;
      }
    }
  }

  .blog-content-post-content {
    margin-top: 5vh;

    .blog-content-post-content-image {
      img {
        width: 60vw;
        border-radius: 10px;
        box-shadow: 5px 5px 5px 5px grey;
        margin-top: 40px;
      }
    }

    .blog-content-post-content-text {
      width: 60vw;
      text-align: left;
      margin: 0 auto;

      h4 {
        font-size: 1.5em;
      }

      p {
        font-weight: 300;
        font-size: 1.2em;
        color: #666;
      }

      button {
        border: none;
        background: transparent;
      }
    }
  }

  .modal-post {
    width: 100%;
    height: 100vh;
    background-color: rgba(133, 128, 111, 0.5);
    backdrop-filter: blur(10px);
    top: 0;
    position: fixed;
    opacity: 10px;
    left: 0;
  }

  .modal-post-display {
    width: 60%;
    height: 90vh;
    border: 1px solid #333;
    background: #eee;
    overflow: auto;
    text-align: left;
    border-radius: 5px;
    position: fixed;
    top: 0;
    margin-left: 22.5%;
    margin-top: 4.5vh;
    font-family: sans-serif;

    p {
      color: #666;
    }

    h4 {
      font-size: 1.2em;
    }

    .modal-post-image {
      display: flex;

      img {
        width: 80%;
        margin: 0 auto;
      }
    }

    .modal-post-display-content {
      margin: 0 15px;

      li {
        line-height: 35px;
      }
    }
  }
}
</style>
