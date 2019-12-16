<template>
  <div class="book">
    <div class="book-tile">
      <h2>Sách</h2>
      <hr />
    </div>
    <div class="book-content">
      <div
        class="book-content-item"
        @click="showModalBook = !showModalBook"
        v-for="(book, index) in allBook"
        :key="`book-${index}`"
      >
        <div class="book-content-item-img">
          <img :src="book.img" alt="" />
        </div>
        <div class="book-content-item-text">
          <p>{{ book.title }}</p>
          <span>{{ book.author }}</span>
          <h4>
            {{ book.price }}<span> {{ book.onSale }}</span>
          </h4>
          <span>{{ book.rate }} {{ book.comment }}</span>
        </div>
      </div>
      <div class="modal" v-if="showModalBook">
        <modal-book v-if="showModalBook"></modal-book>
      </div>
    </div>
  </div>
</template>

<script>
import ModalBook from "@/components/books/modal-book.vue";
import { allBook } from "@/components/books/allBook.js";
export default {
  components: {
    ModalBook
  },
  data() {
    return {
      showModalBook: false,
      allBook
    };
  }
};
</script>

<style lang="scss" scoped>
.book {
  width: 100vw;
  text-align: center;
  font-family: sans-serif;

  .book-tile {
    h2 {
      font-size: 2.7em;
      font-family: monospace;
      font-weight: 300;
    }

    hr {
      width: 80vw;
      margin-top: 10vh;
    }
  }

  .book-content {
    display: flex;
    justify-content: flex-start;

    .book-content-item {
      font-family: cursive;
      width: 20vw;
      margin: 30px 30px;

      .book-content-item-text {
        text-align: left;

        span {
          color: #999;
        }
      }

      &:hover {
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
      }
    }
  }
}
</style>
