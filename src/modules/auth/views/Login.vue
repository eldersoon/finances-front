<template>
  <v-container fill-height fluid id="wrapper">
    <v-layout justify-center align-center>
      <v-flex md5>
        <v-card class="elevation-4">
          <v-toolbar color="#66BB6A">
            <v-toolbar-title>Login</v-toolbar-title>
          </v-toolbar>

          <v-card-text class="card-body">
            <v-form>
              <v-text-field
              prepend-icon="mdi-email"
              name="email"
              type="email"
              label="Email"
              ></v-text-field>

              <v-text-field
              prepend-icon="mdi-lock"
              name="password"
              type="password"
              label="Password"
              ></v-text-field>

              <div class="buttons">
                <v-btn id="btn-large" color="secondary" large>Create account</v-btn>
                <v-btn id="btn-large" color="#66BB6A" large>Enter</v-btn>
              </div>
            </v-form>
          </v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  name: 'Login',
  data: () => {}
}
</script>

<style scoped>
#wrapper {
  background-color: #263238;
}

.card-body {
  background-color: #CFD8DC;
}

#btn-large {
  margin: 0 5px;
}

.buttons {
  display: table;
  margin: 0 auto;
}

input:-webkit-autofill,
input:-webkit-autofill:hover,
input:-webkit-autofill:focus,
input:-webkit-autofill:active  {
  box-shadow: 0 0 0 30px white inset !important;
}
</style>
