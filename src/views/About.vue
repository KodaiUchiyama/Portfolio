<template>
  <v-container
        py-12
        px-5>
        <v-row
            align-content="center">
            <v-col cols="12" sm="12" md="6">
              <v-card tile>
                <a href="https://goo.gl/maps/fjTS6sDtrZ2jfDix9" target="_blank">
                  <v-img
                    src="../assets/fuji.jpg"
                    aspect-ratio="1.7"
                    max-height="350">
                  </v-img>
                </a>
              </v-card>
            </v-col>
            <v-col cols="12" sm="6" md="6">
                <div>
                    <v-card-title primary-title class="py-0">
                            <div class="text-h6 text-xl-h3">{{ myname }}</div>
                            <div class="text-h6 text-xl-h3">{{ sentence }}</div>
                            <div class="text-h6 text-xl-h3 font-italic">{{ jobs }}</div>
                    </v-card-title>
                    <v-card-text class="text-h6">
                        <div>{{ hobby }}</div>
                        <div>Let's make <span class="font-italic font-color-yellow">something</span> great!</div>
                        <a href="mailto:kody.uchiyama@gmail.com" target="_blank" class="font-color-black">{{ address }}</a><span> → for</span>
                        <div>→→→ collaborations.</div>
                    </v-card-text>

                </div>
            </v-col>
        </v-row>
  </v-container>
</template>

<script>
export default {
  data () {
    return {
      myname: 'Hello, My name is Kodai,',
      sentence: 'I am currently working as a',
      jobs: 'Full-stack Web Engineer.',
      hobby: '-',
      great: "Let's make something great!",
      address: 'kody.uchiyama@gmail.com'
    }
  }
}
</script>
<style lang="scss">
.font-color-yellow {
   color: #F9BC08;
}
.font-color-black {
   color: #000 !important;
}
</style>
