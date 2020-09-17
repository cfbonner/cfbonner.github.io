<template>
  <main class='p-6'>
    <h1 class='sr-only'>Work</h1>
    <section class='space-y-8' style='max-width: 75ch;'>
      <ListingEntry
        v-for='entry in entries'
        v-bind:entry='entry'
        v-bind:key='entry.name'
      />
    </section>
  </main>
</template>

<script>
import ListingEntry from '../components/ListingEntry'
export default {
  components: {
    ListingEntry
  },
  data() {
    return {
      entries: [
        {
          id: 1,
          title: 'Agency work',
          subtitle: 'Ruby on Rails, Javascript',
          meta_description: 'I build Ruby on Rails apps everyday at Primate. Lots of them. I started as a front-end developer, bringing the design team\'s vision to life. I primarily focus now on back-end, building donation gateways, accreditation software, CRM integrations, and our custom CMS. We have some pretty cool clients so you should check out our website to see those.'
        },
        {
          id: 2,
          title: 'Flourish Festival',
          subtitle: 'Ruby on Rails',
          meta_description: 'Sometimes we want to hide from ourselves — we do not want to be us — it is too difficult to be us. It is at these times that we turn to drugs or alcohol or behavior to help us forget that we are ourselves.'
        },
        {
          id: 3,
          title: 'Tattler - Chat app',
          subtitle: 'Phoenix, Javascript',
          meta_description: 'Is a dog man’s best friend? I had a dog. The dog was large. It ate my garden, all the plants, and much earth.'
        },
        {
          id: 4,
          title: 'CLI Dungeon Crawler',
          subtitle: 'Elixir',
          meta_description: 'Is a dog man’s best friend? I had a dog. The dog was large. It ate my garden, all the plants, and much earth.'
        },
        {
          id: 5,
          title: 'Log Lady Ipsum',
          subtitle: 'Javascript',
          meta_description: 'Sometimes we want to hide from ourselves — we do not want to be us — it is too difficult to be us. It is at these times that we turn to drugs or alcohol or behavior to help us forget that we are ourselves.'
        },
      ]
    }
  }
}
</script>
