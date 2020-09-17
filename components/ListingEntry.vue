<template>
  <article>
    <h2 class='font-bold'>{{ entry.title }}</h2>
    <p class='italic text-xs mb-2'>{{ entry.subtitle }}</p>
    <p class='text-xs'>{{ entry.meta_description }}</p>
  </article>
</template>

<script>
export default {
  props: [ 'entry' ]
}
</script>

<style></style>
