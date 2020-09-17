<template>
  <nav>
    <ul class="flex flex-wrap space-x-2">
      <li v-for="page in pages" class='text-2xl font-bold text-gray-100'>
        <NuxtLink :to="page.path">{{ page.name }}</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  data() {
    return {
      pages: [
        {
          name: 'About',
          path: '/'
        },
        {
          name: 'Work',
          path: '/work'
        },
        {
          name: 'Contact',
          path: '/contact'
        },
      ]
    }
  },
}
</script>

<style scoped>
.nuxt-link-exact-active {
  text-decoration: underline;
}
</style>
