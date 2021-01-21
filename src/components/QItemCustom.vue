<template>
  <div>
    <q-item v-for="(doctor, index) in doctors" :key="index" clickable class="bg-white full-width q-mb-sm">
      <q-item-section avatar>
        <q-avatar>
          <img :src="doctor.avatar" />
        </q-avatar>
      </q-item-section>

      <q-item-section>
        <q-item-label class="text-items-name text-weight-bold text-items-color2" lines="1">{{ doctor.name }}</q-item-label>
        <q-item-label class="text-items-speciality" caption lines="2">
          {{ doctor.speciality }}
        </q-item-label>
      </q-item-section>

      <q-item-section side>
        <div class="flex items-center">
          <q-icon class="q-pr-xs" name="star" size="12px" color="amber-8" />
          <div class="text-items-ranking text-items-color2 ">{{ doctor.ranking }}</div>
        </div>
      </q-item-section>
    </q-item>
  </div>
</template>
<script>
export default {
  props: {
    doctors: {
      require: true,
      type: Array
    }
  }
}
</script>
<style lang="scss" scoped>
.text-items-color2 {
  color: #132754 !important;
}
.text-items-name {
  font-size: 11px;
}
.text-items-speciality {
  font-size: 10px;
}
.text-items-ranking {
  font-size: 10px;
  font-weight: bold;
}
</style>
