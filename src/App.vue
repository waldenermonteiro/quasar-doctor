<template>
  <div id="q-app">
    <router-view />
  </div>
</template>
<script>
export default {
  name: 'App'
}
</script>
<style>
/* .q-field__label {
  color: #cbd0e0;
  /* opacity: 0.6;
} */
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
