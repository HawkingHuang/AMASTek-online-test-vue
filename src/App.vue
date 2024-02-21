<template>
  <v-app>
    <v-main>
      <Main />
      <Timer />
    </v-main>
  </v-app>
</template>

<script>
import Timer from "./components/Timer";
import Main from "./components/Main";

export default {
  name: "App",

  components: {
    Timer,
    Main,
  },

  data: () => ({
    //
  }),
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  max-width: 1280px;
  margin: 20px auto;
}
</style>
