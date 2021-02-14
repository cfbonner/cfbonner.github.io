<template>
  <article v-if='entry.published'>
    <h2 class='font-bold md:text-xl'>{{ entry.title }}</h2>
    <p class='italic text-base md:text-xl mb-2'>{{ entry.subtitle }}</p>
    <p class='text-base md:text-lg'>{{ entry.meta_description }}</p>
    <footer class='mt-4'>
      <a v-if='entry.url' :href='entry.url' class='cursor-pointer text-base rounded py-1 px-4 bg-yellow-500 text-black hover:bg-pink-500'>{{ entry.link_text }} &#8605;</a>
    </footer>
  </article>
</template>

<script>
export default {
  props: [ 'entry' ]
}
</script>

<style></style>
