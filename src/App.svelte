<script lang="ts">
  import Hero from './lib/Hero.svelte';
  import Navbar from './lib/Navbar.svelte';
  import Tech from './lib/Tech.svelte';
  import Hr from './lib/Hr.svelte';
  import Projects from './lib/Projects.svelte';
  import Footer from './lib/Footer.svelte';
</script>

<main>
  <Navbar />

  <Hero />
  <Hr />

  <Tech />
  <Hr />

  <Projects />
  <Hr />

  <Footer />
</main>

<style>
  :global(:root) {
    --color-accent: #60B8D3;;
    --color-light-grey: #707070;
  }
</style>
