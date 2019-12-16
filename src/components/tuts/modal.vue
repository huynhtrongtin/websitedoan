<template>
  <div class="modal">
    <iframe
      width="50%"
      height="50%"
      src="https://www.youtube.com/embed/slYsupe9FzY"
    ></iframe>
    <div class="button-close">
      <button>X</button>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.modal {
  width: 100%;
  height: 100vh;
  position: fixed;
  top: 0;
  background-color: rgba(133, 128, 111, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
  display: none;

  iframe {
    position: relative;
  }

  .button-close {
    position: absolute;
    text-align: right;

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
</style>
