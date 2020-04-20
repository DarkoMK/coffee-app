<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="fas fa-coffee"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />

        <q-toolbar-title>
        </q-toolbar-title>

        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />
      </q-toolbar>
      <q-card class="bg-primary" flat>
        <q-card-section class="text-center q-pa-none">
          <q-img src="/statics/coffee.png" height="50px" contain></q-img>
          <h6 class="text-h6 text-white q-my-md">Hi, John Snow</h6>
        </q-card-section>
      </q-card>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      content-class="bg-primary"
    >
      <div class="col column">
        <div class="col-6 justify-center content-end">
          <q-img src="/statics/coffee.png" height="100px" class="q-mt-lg" contain></q-img>
        </div>
        <div class="col q-pa-xl">
          <q-list dark>
            <EssentialLink
              v-for="link in essentialLinks"
              :key="link.title"
              v-bind="link"
            />
          </q-list>
        </div>
      </div>
    </q-drawer>

    <q-page-container>
      <router-view/>
    </q-page-container>
  </q-layout>
</template>

<script>
  import EssentialLink from 'components/EssentialLink'

  export default {
    name: 'MainLayout',

    components: {
      EssentialLink
    },

    data() {
      return {
        leftDrawerOpen: false,
        essentialLinks: [
          {
            title: 'New Order',
            icon: 'fas fa-arrow-circle-right',
            link: '/order'
          },
          {
            title: 'My Orders',
            icon: 'fas fa-arrow-circle-right'
          },
          {
            title: 'Help Info',
            icon: 'fas fa-arrow-circle-right'
          },
          {
            title: 'Profile',
            icon: 'fas fa-arrow-circle-right'
          },
          {
            title: 'Payments',
            icon: 'fas fa-arrow-circle-right'
          },
          {
            title: 'Log Out',
            icon: 'fas fa-arrow-circle-right',
            link: '/'
          }
        ]
      }
    }
  }
</script>
