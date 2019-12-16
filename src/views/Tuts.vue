<template>
  <div class="tuts">
    <div class="ms-nav-wrapper">
      <ms-header />
    </div>
    <ms-lesson></ms-lesson>
    <ms-registration></ms-registration>
    <ms-list-lesson></ms-list-lesson>
    <modal></modal>
    <ms-persistence></ms-persistence>
  </div>
</template>

<script>
// @ is an alias to /src
import msHeader from "@/components/header/ms-header.vue";
import msLesson from "@/components/tuts/ms-lesson.vue";
import msRegistration from "@/components/home/ms-registration.vue";
import msListLesson from "@/components/tuts/ms-list-lesson.vue";
import Modal from "@/components/tuts/modal.vue";
import msPersistence from "@/components/tuts/ms-persistence";

export default {
  name: "tuts",
  components: {
    msHeader,
    msLesson,
    msRegistration,
    msListLesson,
    Modal,
    msPersistence
  }
};
</script>
