<template>
  <Suspense>
    <template #fallback>
      <SplashScreen />
    </template>
    <template #default>
      <Home />
    </template>
  </Suspense>
</template>

<script>
import { defineAsyncComponent } from "vue";
import SplashScreen from "./components/SplashScreen.vue";

export default {
  name: 'App',
  components: {
    SplashScreen,
    Home: defineAsyncComponent(() => {
      return new Promise((resol) => {
        setTimeout(() => {
          resol(import("./components/Home.vue"));
        }, 2500);
      });
    }),
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #408ad4;

  
}
* {
  --brand-green: rgb(111, 233, 111);
  --brand-blue: rgb(115, 192, 230);
}
</style>
