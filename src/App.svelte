<script>

    import Header from "./components/Header.svelte";
    import Footer from "./components/Footer.svelte";
    import Assignemnts from "./components/Assignments.svelte";
    import Team from "./components/Team.svelte";
    import Links from "./components/Links.svelte";

</script>


<Header />
<section>
  <Assignemnts />
  <Team />
  <Links />
</section>
<Footer />

<style>

  /* Root for CSS Variables */
  :root {
    --black: #191819;
    --white: #FFFDFD;
    --accent: #1F7A8C;

    --boxShadowDefault: 1px 1px 0px var(--white);
  }

  :global(::selection, ::-moz-selection) {
      color: var(--white);
      background: var(--accent);
  }

  /* Reset Browser Defaults */
  :global(*) {  
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'IBM Plex Mono', monospace;
  }
  
  /* Site-wide padding */
  :global(header), :global(footer), :global(section) {
    padding: 1rem;
  }

  /* Set app to fill as much space as required with header and footer, rest section */
  :global(#app) {
    min-height: 100vh;
    
    display: grid;
    grid-template-rows: auto 1fr auto;
    
    background-color: var(--black);
  }

  :global(h2) {
    color: var(--white);
    font-size: 1.8rem;
  }

  section {
    max-width: 80rem;
    justify-self: center;
  }

</style>