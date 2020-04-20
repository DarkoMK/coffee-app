<template>
  <q-page>
    <q-card class="my-card">
      <img src="/statics/people.jpg">

      <q-list>
        <q-item clickable to="/order">
          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-coffee"/>
          </q-item-section>

          <q-item-section>
            <q-item-label>New Order</q-item-label>
            <q-item-label caption>Take a break!</q-item-label>
          </q-item-section>
        </q-item>

        <q-item clickable>
          <q-item-section avatar>
            <q-icon color="red" name="fas fa-list"/>
          </q-item-section>

          <q-item-section>
            <q-item-label>My Orders</q-item-label>
            <q-item-label caption>List orders.</q-item-label>
          </q-item-section>
        </q-item>

        <q-item clickable>
          <q-item-section avatar>
            <q-icon color="amber" name="fas fa-question"/>
          </q-item-section>

          <q-item-section>
            <q-item-label>Help Info</q-item-label>
            <q-item-label caption>Need help?</q-item-label>
          </q-item-section>
        </q-item>

        <q-item clickable>
          <q-item-section avatar>
            <q-icon color="red" name="fas fa-user"/>
          </q-item-section>

          <q-item-section>
            <q-item-label>Profile</q-item-label>
            <q-item-label caption>Edit profile info.</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>
    </q-card>
  </q-page>
</template>

<script>
  export default {
    name: 'PageIndex'
  }
</script>

<style lang="sass" scoped>
  .my-card
    width: 100%
</style>
