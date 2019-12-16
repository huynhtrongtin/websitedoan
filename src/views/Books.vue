<template>
  <div class="question">
    <div class="ms-nav-wrapper">
      <ms-header />
    </div>
    <page-book></page-book>
  </div>
</template>

<script>
// @ is an alias to /src
import msHeader from "@/components/header/ms-header.vue";
import pageBook from "@/components/books/page-book.vue";

export default {
  name: "book",
  components: {
    msHeader,
    pageBook
  }
};
</script>
