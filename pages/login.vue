<template>
  <v-container>
    <h1>Login</h1>

    <UserAuthForm buttonText="Login" :submitForm="loginUser" />
  </v-container>
</template>

<script>
import UserAuthForm from "@/components/UserAuthForm";
export default {
  components: {
    UserAuthForm
  },
  methods: {
    loginUser(loginInfo) {
      // choose strategy here
      this.$auth.loginWith("local", {
        data: loginInfo,
      });
      /* alert('You pressed a button') */
    }
  }
};
</script>

<style lang="scss" scoped></style>
