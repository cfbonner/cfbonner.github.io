<template>
  <main>
    <section>
      <ul>
        <li v-for='(url, service) in links'>
          <strong>{{ service }}</strong>: {{ url }}
        </li>
      </ul>
    </section>
  </main>
</template>

<script>
export default {
  data() {
    return {
      links: {
        Email: 'cfbonner[at]gmail.com',
        GitHub: 'www.github.com/cfbonner',
      }
    }
  }
}
</script>

<style></style>
