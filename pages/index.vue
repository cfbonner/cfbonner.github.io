<template>
  <main>
    <section class='text-base space-y-3 md:space-y-4 md:text-xl' style='max-width: 65ch;'>
      <p class='font-bold'>
      Hi there.
      </p>
      <p>
      I'm a web developer. Canadian. I live in Scotland.
      </p>
      <p>
      I work at an awesome digital agency called <a href="https://www.primate.co.uk" class='text-yellow-500'>Primate</a>. I also take on freelance work that I find interesting.
      </p>
      <p>
      I get excited about normal web things, like intuitive experiences, blistering fast performance, accessibility, high ranking SEO. Normal web things.
      </p>
      <p>
      I also get excited about strange web things like latent design, useful VIM macros, easter-eggs, keyboard shortcuts, and experimental browser API's.
      </p>
      <p>
      The technology I most often rely on includes but is not limited to:
      </p>
      <ul class="ml-4 space-y-1">
        <li v-for="skill in skills" class="list-disc">
          {{ skill }}
        </li>
      </ul>
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
        'HTML5',
        'CSS/SASS',
      ]
    }
  }
}
</script>

<style></style>
