<template>
  <v-container class="navBar">
    <v-row class="text-center">
      <v-col
        class="mb-5"
        cols="12"
      >
        <v-row justify="center">
          <router-link to="/resume" custom v-slot="{ navigate }">
            <span @click="navigate" role="link">resume</span>
          </router-link>

          <a
            v-for="(next, i) in menuLinks"
            :key="i"
            :href="next.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ next.text }}
          </a>

          <router-link to="/about" custom v-slot="{ navigate }">
            <span @click="navigate" role="link">a bit more about me</span>
          </router-link>

        </v-row>
      </v-col>

    </v-row>
  </v-container>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'navigationBar',

  data () {
    return {
      menuLinks: [
        {
          text: 'linkedIn',
          href: 'https://www.linkedin.com/in/lu-antoine/'
        },
        {
          text: 'github',
          href: 'https://github.com/antoinezl'
        }
      ],
      buttons: [{
        name: 'a bit more about me'
      }]
    }
  }
})
</script>
