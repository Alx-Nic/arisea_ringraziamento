<template>
  <VideoBackground 
  :src="require('@/assets/HeroMobile.mp4')" 
  :sources="[
        {src: '/Hero.mp4', res: 900, autoplay: true}, 
    ]"
  style="height: 100vh;"
  >
    <v-container class="foo fill-height">
      <v-row class="text-center">
        <v-col cols="12">
          <v-img :src="require('../assets/logoArisea.png')" class="my-3" contain height="200" />
        </v-col>

        <v-col cols="12">
          <h1>Grazie !!!</h1>
          <p>per aver partecipato alla festa !</p>
          <p>Anche per te abbiamo un regalo</p>
        </v-col>
        <v-col cols="12">
          <h2>Uno sconto di 10% per oranizare la tua festa perfetta</h2>
        </v-col>
        <v-col cols="12">
          <v-btn @click="navigateToInstagram" color="#f2d1da">riscatta</v-btn>
        </v-col>
        <v-col cols="12">
          <h2>Non perdere l`occasione !</h2>
        </v-col>
      </v-row>
    </v-container>
  </VideoBackground>
</template>

<script>

import VideoBackground from 'vue-responsive-video-background-player'


export default {
  name: "HelloWorld",

  components: { VideoBackground },


  data: () => ({}),
  methods: {
    navigateToInstagram: function () {
      window.location.href = "https://ig.me/m/ariseapartyinstyle";
    },
  },
};
</script>

<style scoped>

</style>
