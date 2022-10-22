<template>
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
  
</template>

<script>
export default {
  name: "HelloWorld",

  data: () => ({}),
  methods: {
    navigateToInstagram: function () {
      window.location.href = "https://ig.me/m/ariseapartyinstyle";
    },
  },
};
</script>

<style scoped>




@media only screen and (min-width: 601px) {
  .foo {
    background: url("@/assets/Hero1200x2133.png");
  }
}

@media only screen and (max-width: 600px) {
  .foo {
    background: url("@/assets/HeroMobile.png");
  }
}


.foo {
  /* background: url("@/assets/1496_BIRTHDAY2.png"); */
  /* background: url("@/assets/HeoMobile.png"); */ 
  /* background: url("@/assets/Hero1200x2133.png"); */
  background-size: cover;
  background-position: center;
  /* background-repeat: no-repeat; */
  height: 100vh;
  /* width: 100vh; */
}




</style>
