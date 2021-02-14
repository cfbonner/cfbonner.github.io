<template>
  <main>
    <section
      class="text-base space-y-3 md:space-y-4 md:text-xl"
      style="max-width: 65ch;"
    >
      <nuxt-content :document="page" class="space-y-4" />
    </section>
  </main>
</template>

<script>
import Navigation from "../components/Navigation";
export default {
  components: {
    Navigation,
  },
  async asyncData({ $content }) {
    const [page] = await $content("pages")
      .where({ title: "About" })
      .fetch();

    return {
      page,
    };
  },
};
</script>
