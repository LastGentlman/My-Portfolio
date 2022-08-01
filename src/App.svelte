<script>
  import { Router, Link, Route } from 'svelte-routing'
  import NotFound from './views/404.svelte'
  import Header from './lib/Header.svelte'
  import Intro from './lib/Intro.svelte'
  import MyServices from './lib/MyServices.svelte'
  import About from './lib/About.svelte'
  import MyProjects from './lib/MyProjects.svelte'
  import Footer from './lib/Footer.svelte'
  import Project01 from './views/project_01.svelte'
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

    <Route path="project01">
      <Project01 />
    </Route>

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