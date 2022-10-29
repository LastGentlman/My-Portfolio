<script>
  import { Router, Link, Route } from 'svelte-routing'
  import NotFound from './views/404.svelte'
  import Header from './lib/Header.svelte'
  import Intro from './lib/Intro.svelte'
  import MyServices from './lib/MyServices.svelte'
  import About from './lib/About.svelte'
  import MyProjects from './lib/MyProjects.svelte'
  import Footer from './lib/Footer.svelte'
  import Project01 from './views/weather.svelte'
  import Project03 from './views/meme.svelte'
  import Project04 from './views/rpsgame.svelte'
  import Project05 from './views/story.svelte'
  import Project06 from './views/recipes.svelte'
</script>

<main>
  
  <Header />

  <Router>
    <Route path="/">
      <Intro />
      <MyServices />
      <About />
      <MyProjects />
      <Footer />
    </Route>

    <Route path="project01"><Project01 /></Route>
    <Route path="project03"><Project03 /></Route>
    <Route path="project04"><Project04 /></Route>
    <Route path="project05"><Project05 /></Route>
    <Route path="project06"><Project06 /></Route>

    <Route path="*">
      <NotFound />
    </Route>
  </Router>

</main>

<style>
  *, main {
    margin: 0;
    padding: 0;
  }
</style>