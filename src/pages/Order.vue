<template>
  <q-page>
    <q-toolbar class="bg-primary text-white">
      <q-btn
        flat
        dense
        round
        icon="fas fa-info-circle"
        aria-label="Info"
      />

      <q-toolbar-title class="text-center">
        New Order
      </q-toolbar-title>

      <q-btn
        flat
        dense
        round
        icon="fas fa-arrow-circle-right"
        aria-label="Home"
        to="/home"
      />
    </q-toolbar>
    <q-card class="my-card">
      <img src="/statics/coffee.png" height="100px" style="object-fit: scale-down">
      <q-card-section class="q-pa-none">
        <q-tabs
          dense
          class="bg-grey-2 text-primary"
        >
          <q-tab name="mails" label="Coffees"/>
          <q-tab name="alarms" label="Cold Brews"/>
          <q-tab name="movies" label="Ice Cream"/>
        </q-tabs>
      </q-card-section>
      <q-list>
        <q-item clickable to="/order/confirm">
          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-coffee"/>
          </q-item-section>

          <q-item-section class="text-center">
            <q-item-label>Americano+</q-item-label>
            <q-item-label caption class="text-primary">$4.25</q-item-label>
          </q-item-section>

          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-shopping-bag"/>
          </q-item-section>
        </q-item>

        <q-item clickable>
          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-coffee"/>
          </q-item-section>

          <q-item-section class="text-center">
            <q-item-label>Cappuchino</q-item-label>
            <q-item-label caption class="text-primary">$6.25</q-item-label>
          </q-item-section>

          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-shopping-bag"/>
          </q-item-section>
        </q-item>

        <q-item clickable>
          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-coffee"/>
          </q-item-section>

          <q-item-section class="text-center">
            <q-item-label>Americano2</q-item-label>
            <q-item-label caption class="text-primary">$4.25</q-item-label>
          </q-item-section>

          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-shopping-bag"/>
          </q-item-section>
        </q-item>

        <q-item clickable>
          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-coffee"/>
          </q-item-section>

          <q-item-section class="text-center">
            <q-item-label>Flat White</q-item-label>
            <q-item-label caption class="text-primary">$9.50</q-item-label>
          </q-item-section>

          <q-item-section avatar>
            <q-icon color="primary" name="fas fa-shopping-bag"/>
          </q-item-section>
        </q-item>
      </q-list>
    </q-card>
  </q-page>
</template>

<script>
  export default {
    name: 'Order'
  }
</script>

<style lang="sass" scoped>
  .my-card
    width: 100%
</style>
