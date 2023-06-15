<template>
  <v-app-bar app color="#112e41" dark flat class="px-12">
    <v-btn color="white">
      <v-icon color="#ff6f00" left class="mr-2">fas fa-signature</v-icon>BSM
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')" color="#ff6f00">Home</v-btn>
    <v-btn text @click="scroll('about')" color="white">About</v-btn>
    <v-btn text @click="scroll('portfolio')" color="white">Portfolio</v-btn>
    <v-btn text @click="scroll('services')" color="white">Services</v-btn>
    <v-btn text @click="scroll('page')" color="white">Page</v-btn>
    <v-btn text @click="scroll('biog')" color="white">Biog</v-btn>
    <v-btn text @click="scroll('contact')" color="white">Contact</v-btn>
  </v-app-bar>
</template>

<script>
export default {
  methods: {
    scroll(refName) {
      const element = document.getElementById(refName);
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style></style>
