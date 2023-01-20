<template>
  <q-layout view="lHh Lpr lFf">
    <GlobalHeader />
    <q-page-container>
      <HelloWorld />
    </q-page-container>
  </q-layout>
</template>

<script>
import { ref } from 'vue'
import HelloWorld from './components/HelloWorld.vue'
import GlobalHeader from './components/GlobalHeader.vue'

export default {
  name: 'LayoutDefault',

  components: {
    GlobalHeader,
    HelloWorld
  },

  setup () {
    return {
      leftDrawerOpen: ref(false)
    }
  }
}
</script>
