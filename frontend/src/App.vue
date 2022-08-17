<template>
  <v-app>
    <v-main id="app-holder">
      <v-header class="d-flex justify-space-between align-center mt-2">
        <Date />
        <Greeting />
        <WeatherWidget city='leeds'/>
      </v-header>
    </v-main>
  </v-app>
</template>

<style>
  *,
  *::before,
  *::after {
      box-sizing: border-box;
  }

  #app-holder {
    width: 1024px;
    height: 600px;
    border-style: dashed;
    border-color: orange;
  }
</style>

<script>

import Date from './components/Date.vue'
import Greeting from './components/Greeting.vue'
import WeatherWidget from './components/WeatherWidget.vue'

export default {
  name: 'App',

  components: {
    Date,
    Greeting,
    WeatherWidget,
  },

  data: () => ({
    //
  }),
}
</script>
