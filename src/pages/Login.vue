<template>
  <q-page class="bg-primary window-height window-width row justify-center">
    <div class="column full-width">
      <div class="col column">
        <div class="col-10">
          <div class="row items-center justify-center" style="height: 100%">
            <q-img src="/statics/coffee.png" height="80%" contain></q-img>
          </div>
        </div>
        <div class="col">
          <div class="row items-end justify-center" style="height: 100%">
            <h5 class="text-h5 text-white q-my-md">Coffee Shop System</h5>
          </div>
        </div>
      </div>
      <div class="col">
        <q-card class="full-height full-width q-pa-sm" flat square>
          <q-card-section>
            <q-form class="q-gutter-md">
              <q-input square filled clearable v-model="username" type="text" label="Username"/>
              <q-input square filled clearable v-model="password" type="password" label="Password"/>
            </q-form>
          </q-card-section>
          <q-card-actions class="q-px-md">
            <q-btn unelevated color="primary" size="lg" class="full-width" label="Log in" to="home" />
          </q-card-actions>
          <q-card-section class="text-center q-pa-none">
            <q-img src="/statics/iced-coffee.png" height="50px" contain></q-img>
            <p class="text-primary">Forgot your password?</p>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </q-page>
</template>

<script>
  export default {
    name: "Login",
    data() {
      return {
        username: '',
        password: ''
      }
    }
  }
</script>

<style scoped>

</style>
