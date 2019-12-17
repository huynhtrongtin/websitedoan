<template>
  <div class="modal-book">
    <div
      class="modal-book-background"
      @click="handleCloseModal"
    ></div>
    <div class="modal-book-item">
      <div class="modal-book-item-img">
        <img :src="book.img" alt="" />
      </div>
      <div class="modal-book-content">
        <h2>{{ book.title }}</h2>
        <p>{{ book.rate}} {{ book.comment }}</p>
        <span>Tác giả: {{ book.author }} </span>
        <span style="font-weight: bold;margin-left: 5vw;">Bìa mềm</span>
        <p>Id: {{ book.id }}</p>
        <hr />
        <h3 style="color: red;">{{ book.price }}</h3>
        <p>
          Tiết kiệm: <span style="color: red;">{{ book.onSale }} </span><span>({{ book.priceOnSale }})</span>
        </p>
        <p>Giá thị trường: {{ book.marketPrice }}</p>
        <hr />
        <div class="total-book">
          <button @click="countBookUpcrease">+</button>
          <p>{{ count }}</p>
          <button @click="countBookDecrease">-</button>
        </div>
        <div class="book-buy">
          <a
            :href="book.link"
            target="_blank"
            ><button><i class="fas fa-shopping-cart"></i>Chọn mua</button></a
          >
          <span @click="showHeartIcon = !showHeartIcon">
            <i class="far fa-heart" id="heart-icon" v-if="!showHeartIcon"></i>
            <i
              class="fas fa-heart"
              id="heart-icon"
              style="color:#ff3945;"
              v-if="showHeartIcon"
            ></i>
          </span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    book: {
      type: Object,
    }
  },
  data() {
    return {
      count: 1,
      showHeartIcon: false,
    };
  },
  methods: {
    countBookUpcrease: function() {
      this.count += 1;
    },
    countBookDecrease: function() {
      this.count -= 1;
    },
    handleCloseModal() {
      this.$emit('close')
    }
  }
};
</script>

<style lang="scss" scoped>
.modal-book {
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
  position: fixed;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: cursive;
  .modal-book-background {
    top: 0;
    left: 0;
    width: 100%;
    height: 100vh;
    position: fixed;
    display: flex;
    justify-content: center;
    align-items: center;
    font-family: cursive;
    background-color: rgba(133, 128, 111, 0.5);
  }
  .modal-book-item {
    width: 80%;
    height: 80vh;
    margin: 0 auto;
    background-color: #fff;
    display: flex;
    position: relative;
    .modal-book-item-img {
      height: 88%;
      margin: 5vh 3vw 0 3vw;
      border-right: 1px solid #333;
      padding-right: 5vw;
    }
    .modal-book-content {
      text-align: left;
      margin-top: 5vh;
      hr {
        width: 55vw;
        margin-left: -3vw;
      }
    }
    .total-book {
      width: 5.8vw;
      display: flex;
      border: 1px solid #999;
      margin-right: 10vw;
      button {
        height: 3.5vh;
        border-top: none;
        border-bottom: none;
      }
      p {
        height: 3.5vh;
        margin: 0 1vw;
        margin-top: auto;
      }
    }
    .book-buy {
      margin-left: 16vw;
      button {
        width: 20vw;
        height: 7vh;
        border: none;
        border-radius: 5px;
        background-color: #ff3945;
        font-size: 1.2em;
        color: #fff;
        &:hover {
          opacity: 0.8;
        }
        i {
          margin-right: 1vw;
        }
      }
      #heart-icon {
        margin-left: 3vw;
        font-size: 2em;
        color: #999;
        &:hover {
          color: #ff3945;
        }
      }
    }
  }
  .modal-background {
    width: 100%;
  }
}
</style>