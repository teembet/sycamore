<template>
  <v-app>
    <v-app-bar
      app
      color="white"
      style="padding:0 50px 0 50px;"
      dark
      elevation="28"
    >
      <img width="150" src="./assets/site-logo.png" alt="" />
      <v-spacer></v-spacer>

      <v-btn
        target="_blank"
        text
        style="text-transform:none;color:black;font-weight:bold;"
        dark
      >
        About Us
      </v-btn>
      <v-btn
        target="_blank"
        text
        style="text-transform:none;color:black;font-weight:bold;"
        dark
      >
        Contact Us
      </v-btn>
      <v-btn
        target="_blank"
        text
        style="text-transform:none;color:black;font-weight:bold;"
        dark
      >
        Food Store
      </v-btn>
      <v-btn
        target="_blank"
        text
        style="text-transform:none;color:black;font-weight:bold;"
        dark
      >
        Blog
      </v-btn>
      <v-btn
        depressed
        style=" text-transform:none;border-radius:20px;margin-left:100px;"
        dark
        color="#63C132"
        >Login
        <v-icon style="margin-left:10px;font-size:13px" dark
          >mdi-arrow-right</v-icon
        ></v-btn
      >
    </v-app-bar>

    <v-main>
      <!-- <HelloWorld /> -->

      <app-home></app-home>
      <app-footer></app-footer>
    </v-main>
  </v-app>
</template>

<script>
// import HelloWorld from "./components/HelloWorld";
import home from "./components/home";

import footer from "./components/footer";
export default {
  name: "App",

  components: {
    "app-home": home,

    "app-footer": footer,
  },

  data: () => ({
    //
  }),
};
</script>
<style scoped>
.myapp {
  font-family: "Poppins", sans-serif;
}
</style>
