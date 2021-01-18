<template>
  <div class="q-px-md q-pt-md">
    <div class="column container--signup">
      <div class="col-12 q-px-sm q-py-lg">
        <div class="float-left absolute">
          <q-icon class="float-left" name="menu" color="white" size="sm" />
        </div>
        <div class="">
          <q-icon class="float-right" name="mdi-account" color="white" size="sm" />
        </div>
      </div>
      <div class="col-12 q-px-sm q-pb-md">
        <div class="text-h5 text-weight-bold text-white">
          Let's Find Your <br />
          Doctor
        </div>
      </div>
      <div class="col-12 q-px-sm q-pb-md">
        <q-input rounded outlined v-model="search" placeholder="Search Here" dense bg-color="white">
          <template v-slot:append>
            <q-icon name="search" color="" />
          </template>
        </q-input>
      </div>
      <div class="column full-width">
        <div class="form--login__bgcolor q-pa-md" style="height: 82vh !important"></div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      search: ''
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
