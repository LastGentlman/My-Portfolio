<script>
  import Header from './lib/Header.svelte'
  import Intro from './lib/Intro.svelte'
  import MyServices from './lib/MyServices.svelte'
  import About from './lib/About.svelte'
  import MyProjects from './lib/MyProjects.svelte'
  import Footer from './lib/Footer.svelte'
</script>

<main>
  <Header />
  <Intro />
  <MyServices />
  <About />
  <MyProjects />
  <Footer />
</main>

<style>
  *, main {
    margin: 0;
    padding: 0;
  }
</style>