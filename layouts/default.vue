<template>
  <div
    class="px-4 py-8 md:px-32 md:py-16 text-gray-100 min-h-screen"
    style="background-color: #1a1a1a;"
  >
    <header>
      <p class="text-xs md:text-lg text-gray-100">Colin Bonner</p>
      <div class="mb-4 md:mb-8">
        <Navigation />
      </div>
    </header>
    <Nuxt />
  </div>
</template>

<script>
import Navigation from "../components/Navigation";
export default {
  components: {
    Navigation,
  },
};
</script>

<style>
html {
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0;
}
</style>
