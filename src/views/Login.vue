<template>
  <div class="login">
    <login-form></login-form>
  </div>
</template>

<script>
// @ is an alias to /src
import loginForm from "@/components/login/login-form.vue";

export default {
  name: "login",
  components: {
    loginForm
  }
};
</script>

<style>
body {
  overflow: hidden;
}
</style>
