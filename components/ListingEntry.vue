<template>
  <article v-if='entry.published'>
    <h2 class='font-bold'>{{ entry.title }}</h2>
    <p class='italic text-base mb-2'>{{ entry.subtitle }}</p>
    <p class='text-sm'>{{ entry.meta_description }}</p>
    <footer class='mt-2'>
      <a v-if='entry.url' :href='entry.url' class='cursor-pointer text-xs rounded py-1 px-2 bg-yellow-500 text-black'>{{ entry.link_text }}</a>
    </footer>
  </article>
</template>

<script>
export default {
  props: [ 'entry' ]
}
</script>

<style></style>
