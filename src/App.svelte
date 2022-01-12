<script>

    import Assignment from "./components/Assignment.svelte";
    import Header from "./components/Header.svelte";
    import Footer from "./components/Footer.svelte";

</script>


<Header />
<section>

</section>
<Footer />

<style>

  /* Root for CSS Variables */
  :root {
    --black: #343233;
    --white: #FFFDFD;
    --accent: #F98948;
  }

  /* Reset Browser Defaults */
  :global(*) {  
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'roboto';
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

</style>