<script>
  let navToggle;
  let nav;
  let hamburger;
  let flag = false;
  let hamAfter;
  let hamBefore;
  let root = getComputedStyle(document.documentElement)
  let dark = root.getPropertyValue('--clr-dark')
  let light = root.getPropertyValue('--clr-light')  

  function toggle() {
    flag = !flag
    if (flag) {
      nav.style.transform = "translateX(0)"
      hamburger.style.transform = "rotate(.625turn)"
      navToggle.style.position = "fixed"
      hamBefore.style.transform = "rotate(135deg) translate(6px)"
      hamBefore.style.marginLeft = "16px"
      hamBefore.style.marginTop = "3px"
      hamAfter.style.opacity = "0";
      hamburger.style.backgroundColor = light
      hamBefore.style.backgroundColor = light
      hamAfter.style.backgroundColor = light
    } else {
      nav.style.transform = "translateX(100%)"
      hamburger.style.transform = "rotate(0)"
      navToggle.style.position = "absolute"
      hamBefore.style.transform = "rotate(0deg)"
      hamBefore.style.margin = "0 auto"
      hamAfter.style.opacity = "100";
      hamburger.style.backgroundColor = dark
      hamBefore.style.backgroundColor = dark
      hamAfter.style.backgroundColor = dark
    }
  }
</script>

<header>
    <div class="logo">
      <div>{"<Ing-Roy/>"}</div>
    </div>
    
    <button bind:this={navToggle} on:click={toggle} class="nav-toggle" aria-label="Toggle navigation">
      <span bind:this={hamAfter} class="ham-after"></span>
      <span bind:this={hamburger} class="hamburger"></span>
      <span bind:this={hamBefore} class="ham-before"></span>
    </button>
    
  <nav bind:this={nav}>
    <ul class="nav__list">
        <li class="nav__li">
          <a on:click={toggle} href="/" class="nav__link">
            Home
          </a>
        </li>
        <li class="nav__li">
          <a on:click={toggle} href="/#services" class="nav__link">
            My Services
          </a>
        </li>
        <li class="nav__li">
          <a on:click={toggle} href="/#about" class="nav__link">
            About me
          </a>
        </li>
        <li class="nav__li">
          <a on:click={toggle} href="https://ingroy.blogspot.com" target="_blank" class="nav__link">
            My Blog
          </a>
        </li>
        <li class="nav__li">
          <a on:click={toggle} href="/#projects" class="nav__link">
            My Projects
          </a>
        </li>
    </ul>
  </nav>
</header>

<style>
  header {
    display: flex;
    justify-content: space-between;
    padding: 1em;
  }

  .logo {
    max-width: 50vh;
    font-family: var(--ff-secondary);
    font-weight: var(--fw-reg);
    color: var(--clr-label);
    background: var(--clr-light);
    padding: 0 0.125em;
    margin: 0;
    border: 1px solid var(--clr-label);
    border-radius: 0.5em;
  }

  nav {
    position: fixed;
    background: var(--clr-dark);
    color: var(--clr-light);
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    z-index: 100;

    transform: translateX(100%);
    transition: transform 250ms cubic-bezier(.5, 0, .5, 1);
  }

  .nav__list {
    display: flex;
    align-items: center;
    height: 100%;
    flex-direction: column;
    justify-content: space-evenly;
    list-style: none;
  }

  .nav__link {
    color: inherit;
    font-weight: var(--fw-bold);
    font-size: var(--fs-h2);
  }

  .nav__link:hover {
    color: var(--clr-label);
  }

  /* Hamburger menu
  // .nav-open esta en app.css */
  
  .nav-toggle {
    background: transparent;
    border: none;
    cursor: pointer;
    position: absolute;
    padding: .8em;
    right: 1em;
    top: 1em;
    z-index: 1000;
  }

  .hamburger {
    display: block;
    position: relative;
  }

  .hamburger, .ham-after, .ham-before {
    background: var(--clr-dark);
    width: 2em;
    height: 3px;
    border-radius: 1em;
    transition: transform 250ms ease-in-out;
  }

  .ham-before, .ham-after {
    content: "";
    position: absolute;
    left: 0;
    right: 0;
  }

  .ham-before {
    top: 6px;
    margin: 0 auto;
  }

  .ham-after {
    bottom: 6px;
    margin: 0 auto;
  }

</style>