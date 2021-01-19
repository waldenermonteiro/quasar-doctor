<template>
  <div class="q-px-md q-pt-md">
    <div class="row container--signup">
      <div class="col-12 q-px-sm q-py-lg">
        <div class="float-left absolute">
          <q-icon class="float-left" name="menu" color="white" size="sm" />
        </div>
        <div class="">
          <q-icon class="float-right" name="mdi-account" color="white" size="sm" />
        </div>
      </div>
      <div class="col-12 q-px-md q-pb-md row">
        <div class="col-12 q-pb-md">
          <div class="text-h5 text-weight-bold text-white">
            Let's Find Your <br />
            Doctor
          </div>
        </div>
        <div class="col-12 q-pb-md">
          <q-input class="rounded-borders" outlined v-model="search" placeholder="Search Here" dense bg-color="white">
            <template v-slot:append>
              <q-icon name="search" color="" />
            </template>
          </q-input>
        </div>
        <div class="col-3 column items-center">
          <div class="column"><q-avatar color="white" text-color="deep-orange-5" icon="mdi-eye" /></div>
          <div class="column"><p class="circle--text text-grey q-mt-sm">Eye</p></div>
        </div>
        <div class="col-3 column items-center">
          <div class="column"><q-avatar color="white" text-color="info" icon="mdi-heart-pulse" /></div>
          <div class="column"><p class="circle--text text-grey q-mt-sm">Heart</p></div>
        </div>
        <div class="col-3 column items-center">
          <div class="column"><q-avatar color="white" text-color="purple" icon="warning" /></div>
          <div class="column"><p class="circle--text text-grey q-mt-sm">Nose</p></div>
        </div>
        <div class="col-3 column items-center">
          <div class="column"><q-avatar color="white" text-color="secondary" icon="mdi-widgets-outline" /></div>
          <div class="column"><p class="circle--text text-secondary text-teal-12 q-mt-sm">See All</p></div>
        </div>
      </div>
      <div class="column full-width">
        <div class="form--login__bgcolor row">
          <p class=" q-px-md q-pt-md text-weight-bolder text-blue-grey-9">Top Doctors</p>
          <q-list class="rounded-borders full-width q-px-md q-pb-md">
            <q-item clickable class="bg-white full-width q-mb-sm">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label lines="1">Dr Junior Monteiro</q-item-label>
                <q-item-label caption lines="2">
                  <span class="">Heart Surgon</span>
                </q-item-label>
              </q-item-section>

              <q-item-section side>
                <div class="flex items-center">
                  <q-icon class="q-pr-xs" name="star" size="12px" color="amber-8" />
                  <div class="">4.5</div>
                </div>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple class="bg-white full-width q-mb-sm">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label lines="1">Dra Bianca Corrêa</q-item-label>
                <q-item-label caption lines="2">
                  <span class="">Heart Surgon</span>
                </q-item-label>
              </q-item-section>

              <q-item-section side>
                <div class="flex items-center">
                  <q-icon class="q-pr-xs" name="star" size="12px" color="amber-8" />
                  <div>4.5</div>
                </div>
              </q-item-section>
            </q-item>
            <q-item clickable v-ripple class="bg-white full-width q-mb-sm">
              <q-item-section avatar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
                </q-avatar>
              </q-item-section>

              <q-item-section>
                <q-item-label lines="1">Dra Bianca Corrêa</q-item-label>
                <q-item-label caption lines="2">
                  <span class="">Heart Surgon</span>
                </q-item-label>
              </q-item-section>

              <q-item-section side>
                <div class="flex items-center">
                  <q-icon class="q-pr-xs" name="star" size="12px" color="amber-8" />
                  <div>4.5</div>
                </div>
              </q-item-section>
            </q-item>
          </q-list>
        </div>
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
<style lang="scss" scoped>
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
.circle--text {
  font-size: 13px;
  opacity: 0.7;
}
</style>
