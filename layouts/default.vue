<template>
  <div class='font-mono text-gray-100 bg-gray-900 min-h-screen'>
    <header class='p-6'>
      <p class='text-xs text-gray-100'>Colin Bonner</p>
      <Navigation />
    </header>
    <Nuxt />
  </div>
</template>

<script>
import Navigation from '../components/Navigation'
export default {
  components: {
    Navigation
  }
}
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
