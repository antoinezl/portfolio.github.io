<template>
  <v-container>
    <v-row class="text-center">
      <v-col class="mb-5" cols="12">
        <v-container class="mainContainer">
          <v-container class="polaroidFrame flex-rectangle">
            <figure>
              <div id="polaroidBackGround">
                <img :src="require(`../assets/images/profilepic.png`)"
                  alt="ProfilePic"
                  title="It's me, hi!"
                  />
              </div>
              <figcaption>
                <ul>
                  <li>Antoine</li>
                  <li>Lu</li>
                </ul>
              </figcaption>
            </figure>
          </v-container>
        </v-container>
      </v-col>
    </v-row>
  </v-container>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'PolaroidFrame',

  data () {
    return {}
  }
})
</script>
