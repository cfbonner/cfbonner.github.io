<template>
  <nav>
    <ul class="flex flex-col">
      <li>
        <NuxtLink to="/">Home page</NuxtLink>
      </li>
      <li>
        <NuxtLink to="/blog">Blog page</NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
.nuxt-link-exact-active {
  text-decoration: underline;
}

</style>
