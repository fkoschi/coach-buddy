<template>
  <v-container>
    <h1>Register</h1>

    <UserAuthForm buttonText="Register" :submitForm="loginUser" hasName="true"/>
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
      debugger
      alert('You pressed a button')
    }
  }
};
</script>

<style lang="scss" scoped></style>
