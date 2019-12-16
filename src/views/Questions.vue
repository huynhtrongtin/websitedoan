<template>
  <div class="question">
    <div class="ms-nav-wrapper">
      <ms-header />
    </div>
    <page-question></page-question>
  </div>
</template>

<script>
// @ is an alias to /src
import msHeader from "@/components/header/ms-header.vue";
import PageQuestion from "@/components/question/page-question.vue";

export default {
  name: "question",
  components: {
    msHeader,
    PageQuestion
  }
};
</script>
