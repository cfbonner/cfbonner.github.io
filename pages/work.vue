<template>
  <main>
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
          meta_description: 'I build Ruby on Rails apps everyday at Primate. Lots of them. I started as a front-end developer, bringing the design team\'s vision to life. Nowadays I primarily focus on back-end: building donation gateways, accreditation software, CRM integrations, and our custom CMS. We have some pretty cool clients so you should check out our website to see those.',
          link_text: 'primate.co.uk',
          url: 'https://www.primate.co.uk',
          published: true
        },
        {
          id: 2,
          title: 'Flourish Festival',
          subtitle: 'Ruby on Rails, Javascript, Design',
          meta_description: 'This is a site for a grass roots Canadian music/arts festival. It uses an ActiveAdmin powered CMS that the organizers use to manage different interations of the festival, accept applications, create artists from those applications, and add them to a event and schedule builder. Under the cute exterior there\'s some pretty powerful stuff going on.',
          link_text: 'flourish-fest.com',
          url: 'https://www.flourish-fest.com',
          published: true
        },
        {
          id: 4,
          title: 'Cellarghost - music player',
          subtitle: 'Vue, Javascript, Design',
          meta_description: 'This is a music player app that lets you sift through and play from collections of tunes. I used my old band\'s music as a way for us to host our records on our own terms. I\'m hoping to integrate this into a full fledged music app eventually.',
          link_text: 'lucylucylucy.netlify.app',
          url: 'https://lucylucylucy.netlify.app',
          published: true
        },
        {
          id: 7,
          title: 'Lofter',
          subtitle: 'Elixir, Phoenix',
          meta_description: 'There\'s free pitch-and-putt golf course near my house in Edinburgh. I made this LiveView application so that I could track the scores of my fellow Brunstfield Links golfers.',
          link_text: 'lofter.herokuapp.com',
          url: 'https://lofter.herokuapp.com',
          published: true
        },
        {
          id: 5,
          title: 'CLI Dungeon Crawler',
          subtitle: 'Elixir, Mix',
          meta_description: 'The direct result of pandemic lockdown, this is a command line dungeon crawler game where a player moves through rooms looking for a way out, battling enemies and finding items on the way. Written in a functional paradigm using Elixir. It\'s massively geeky in a lot of ways, I guess.',
          published: true,
          link_text: 'github.com/cfbonner/dungeon_crawler',
          url: 'https://github.com/cfbonner/dungeon_crawler',
        },
        {
          id: 3,
          title: 'Tattler - Chat app',
          subtitle: 'Phoenix, Javascript',
          meta_description: 'My take on a standard entry level Elixir/Phoenix app. You can generate a chatroom at any /chat endpoint, send the link to some safe internet friends and chat away.',
          link_text: 'tattlr.herokuapp.com',
          url: 'https://tattlr.herokuapp.com/',
          published: true
        },
        {
          id: 6,
          title: 'Log Lady Ipsum',
          subtitle: 'Phoenix, Javascript',
          meta_description: 'Graciously serves up Twin Peaks\' Log Lady monologues from an API written in Elixir/Phoenix and consumed in a Nuxt.js app. I need placeholder text quite often in my line of work, and I love Twin Peaks so this was pretty necessary after the site I used to use (damngoodcoffeeipsum.com I think?) went offline.',
          link_text: 'logladyipsum.netlify.app',
          url: 'https://logladyipsum.netlify.app/',
          published: false
        },
      ]
    }
  }
}
</script>
