<template>
  <main>
    <h1 class="sr-only">Work</h1>
    <section class="space-y-8" style="max-width: 75ch;">
      <ListingEntry
        v-for="entry in entries"
        v-bind:entry="entry"
        v-bind:key="entry.name"
      />
    </section>
  </main>
</template>

<script>
import ListingEntry from "../components/ListingEntry";
export default {
  components: {
    ListingEntry,
  },
  async asyncData({ $content }) {
    const entries = await $content("work").fetch();

    return {
      entries,
    };
  },
};
</script>
