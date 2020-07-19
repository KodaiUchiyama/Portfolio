<template>
  <v-app>
    <!--<v-app-bar flat color="primary lighten-5" app>-->
    <v-app-bar flat elevate-on-scroll color="shades white" app class="pt-10" style="padding-bottom:90px;">
      <v-img
        class="mx-2"
        src="./assets/logo.png"
        max-height="70"
        max-width="70"
        contain
        style="margin: 0 auto;">
      </v-img>
      <v-toolbar-title style="cursor:pointer;" @click="$router.push('/').catch(()=>{})" class="mx-2 font-weight-medium hidden-xs-only">Kodai Uchiyama</v-toolbar-title>

      <v-spacer></v-spacer>

        <v-btn class="text-none" text tile to="/" id="">Work</v-btn>
        <v-btn class="text-none" text tile to="/about" id="">About</v-btn>
    </v-app-bar>

    <v-main class="my-7">
      <router-view />
    </v-main>

  </v-app>
</template>

<script>
export default {
}
</script>
<style lang="scss">
#no-background-hover::before {
   background-color: transparent !important;
}
</style>
