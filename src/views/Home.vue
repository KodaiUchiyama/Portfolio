<template>

  <v-row justify="center" class="pt-10 mx-3">
    <v-col cols="12" sm="6">
      <v-hover v-slot:default="{ hover }">
        <v-card tile>
          <v-img
            src="../assets/untorn.png"
            aspect-ratio="1.7">
          <v-fade-transition>
            <v-card tile
              v-if="hover"
              class="d-flex justify-center align-center orange darken-2 white--text title"
              target="_blank"
              href="https://untrn.com"
              style="height:100%;">
              <div>UNTORN</div>
            </v-card>
          </v-fade-transition>
          </v-img>
        </v-card>
      </v-hover>
    </v-col>

    <v-col cols="12" sm="6">
      <v-hover v-slot:default="{ hover }">
        <v-card tile>
          <v-img
            src="../assets/D51.jpg"
            aspect-ratio="1.7">
          <v-fade-transition>
            <v-card tile
              v-if="hover"
              class="d-flex justify-center align-center transition-fast-in-fast-out orange darken-2 v-card--reveal white--text title"
              target="_blank"
              href="https://trainart-collection.myshopify.com/"
              style="height:100%;">
              <div>Train Art Collection</div>
            </v-card>
          </v-fade-transition>
          </v-img>
        </v-card>
      </v-hover>
    </v-col>

    <Project />

  </v-row>
</template>

<script>
// @ is an alias to /src
import Project from '@/components/Project.vue'

export default {
  components: {
    Project
  }
}
</script>
<style>
</style>
