<template>
  <q-layout style="background-color:#D6D8EA">
    <Navbar/>
    <!-- <HomeView/> -->
   <router-view/>
  </q-layout>
</template>

<script>
import { ref } from 'vue'
import Navbar from './components/Navbar.vue'
// import HomeView from './views/HomeView.vue'

export default {
  name: 'LayoutDefault',

  components: {
    Navbar,
    // HomeView
  },

  setup () {
    return {
      leftDrawerOpen: ref(false)
    }
  }
}
</script>
