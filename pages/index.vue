<template>
  <main class='p-6'>
    <section class='text-xs space-y-3' style='max-width: 75ch;'>
      <p class='text-base font-bold'>
      Hi there.
      </p>
      <p>
      I'm a web developer. Canadian. I live in Scotland.
      </p>
      <p>
      I work at an awesome digital agency called <a href="https://www.primate.co.uk" class='text-yellow-500'>Primate</a>. I also take on freelance work that I find interesting.
      </p>
      <p>
      I get excited about normal web things, like intuitive experiences, blistering fast performance, accessibility best-practices, high ranking SEO. Normal web things.
      </p>
      <p>
      I also get excited about strange web things like latent design, VIM macros, easter-eggs, keyboard shortcuts, and experimental browser API's.
      </p>
      <p>
      In terms of technologies I use in production, I rely on:
      </p>
      <ul>
        <li v-for="skill in skills" class="list-disc pl-3 ml-3">
          {{ skill }}
        </li>
      </ul>
      <p>
      The mystery of the woods. The woods surrounding Twin Peaks. To introduce this story, let me just say it encompasses the all – it is beyond the “fire”, though few would know that meaning. It is a story of many, but begins with one – and I knew her. The one leading to the many is Laura Palmer. Laura is the one.
      </p>
    </section>
  </main>
</template>

<script>
import Navigation from '../components/Navigation'
export default {
  components: {
    Navigation
  },
  data() {
    return {
      skills: [
        'Ruby/Ruby on Rails',
        'Elixir/Phoenix',
        'Javascript (Vanilla, Vue, React, Stimulus)',
        'HTML (oh yeah, beautiful and semantic)',
        'CSS/SASS',
      ]
    }
  }
}
</script>

<style></style>
