<template>
  <div class="q-px-md q-pt-md" style="height: 100vh">
    <div class="row container--signup">
      <div class="col-12 q-px-sm q-py-lg">
        <div class="float-left absolute">
          <q-icon
            class="float-left"
            name="mdi-chevron-left"
            color="white"
            size="md"
          />
        </div>
        <div class="text-center text-subtitle1 text-weight-regular text-white">
          Sign Up
        </div>
      </div>
      <div class="column full-width">
        <div class="form--login__bgcolor q-pa-md">
          <div class="col-12 q-py-md test">
            <q-input v-model="login" label="Username" dense />
          </div>
          <div class="col-12 q-py-md">
            <q-input v-model="login" label="Password" dense />
          </div>
          <div class="col-12 q-py-md">
            <q-input v-model="login" label="Username" dense />
          </div>
          <div class="col-12 q-py-md">
            <q-input v-model="login" label="Password" dense />
          </div>
          <div class="col-12 row q-py-xl">
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
                class=" btn--login btn--facebook full-width"
                outline
                color="indigo"
                icon="fab fa-facebook-square"
                label="Connect with Facebook"
                rounded
              />
            </div>
          </div>
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
<style scoped>
.container--signup {
  background-color: #555fd2 !important;
  border-radius: 32px !important;
}
.form--login__bgcolor {
  background-color: rgb(239, 244, 251) !important;
  border-radius: 32px !important;
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
</style>
