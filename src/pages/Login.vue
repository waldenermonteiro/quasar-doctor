<template>
  <div class="row q-px-md q-pt-md" style="height: 100vh">
    <div class="column">
      <img
        class=""
        src="../assets/login-image.png"
        width="288px"
        height="100%"
        style="border-radius: 8% 8% 0 0 !important;"
      />
    </div>
    <div class="column full-width">
      <div class="form--login__bgcolor q-pa-md row ">
        <div class="col-12 q-py-md">
          <q-input v-model="login" label="Username" dense />
        </div>
        <div class="col-12 q-py-md">
          <q-input v-model="login" label="Password" dense />
        </div>
        <div class="col-12 q-py-md text--password__size text-white float-right">
          <p class="float-right">Forgot your password ?</p>
        </div>
        <div class="col-12 q-pb-md">
          <q-btn
            class="btn--login btn--signin__bgcolor full-width"
            color="secondary"
            label="SIGN IN"
            rounded
          />
        </div>
        <div class="col-12 q-pb-md">
          <q-btn
            no-caps
            class=" btn--login full-width"
            outline
            color="white"
            icon="fab fa-facebook-square"
            label="Connect with Facebook"
            rounded
          />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      login: '',
      password: ''
    }
  }
}
</script>
<style>
.form--login__bgcolor {
  background-color: #555fd2 !important;
  border-radius: 0 0 8% 8% !important;
}
.text--password__size {
  font-size: 12px;
  font-weight: 300;
}
.btn--signin__bgcolor {
  background-color: #4ce5b1 !important;
}
.btn--login {
  font-size: 12px !important;
  padding: 5px;
}
.q-field__label {
  color: #cbd0e0;
  opacity: 0.6;
}
.q-field__control {
  color: #cbd0e0 !important;
  opacity: 0.6;
  height: 20px;
}
.q-field--standard .q-field__control:before {
  border-color: #cbd0e0 !important;
  opacity: 0.6 !important;
}
</style>
