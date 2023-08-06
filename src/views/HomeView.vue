<template>
  <IntroHeader />
  <PolaroidFrame />
  <NavBar />
</template>

<script lang="ts">
import { defineComponent } from 'vue'

// Components
import IntroHeader from '../components/IntroHeader.vue'
import PolaroidFrame from '../components/PolaroidFrame.vue'
import NavBar from '../components/NavigationBar.vue'

export default defineComponent({
  name: 'HomeView',
  components: {
    IntroHeader,
    PolaroidFrame,
    NavBar
  }
})

</script>
