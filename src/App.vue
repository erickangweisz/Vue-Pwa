<template>
  <v-app>
    <Toolbar/>

    <v-content>
      <MainContent/>
    </v-content>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue'
import MainContent from './components/MainContent.vue'
import Toolbar from '../src/components/Toolbar.vue'

export default Vue.extend({
  name: 'App',

  components: {
    MainContent,
    Toolbar
  },

  data: () => ({
    
  })
})
</script>