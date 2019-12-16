<template>
  <div class="blogs">
    <div class="ms-nav-wrapper">
      <ms-header />
    </div>
    <ms-code-blog></ms-code-blog>
    <blog-content></blog-content>
  </div>
</template>

<script>
import msHeader from "@/components/header/ms-header.vue";
import msCodeBlog from "@/components/blog/ms-code-blog.vue";
import blogContent from "@/components/blog/blog-content.vue";
export default {
  name: "blogs",
  components: {
    msHeader,
    msCodeBlog,
    blogContent
  }
};
</script>
