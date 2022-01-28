<script>
  export let title
</script>


<section>
  <h2>{title}</h2>
  <ul>
    <slot />
  </ul>
</section>

<style>
  
  h2 {
    color: var(--white);
    font-size: 1.8rem;
    margin-bottom: 1rem;
  }

  ul {
    list-style: none;
    width: 100%;
    
    display: grid;
    grid-template-columns: repeat(3, 1fr);

    gap: 1rem;

    position: relative;
  }

  @media only screen and (max-width: 1100px) {
      ul {
          grid-template-columns: 1fr;
      }
  }
  
</style>