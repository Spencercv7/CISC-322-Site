<script>
  export let title
</script>

<style>
  h2 {
    color: var(--white);
    font-size: 1.8rem;
    margin-bottom: 1rem;
  }
  div {
    margin-bottom: 3rem;
  }
</style>

<div>
  <h2>{title}</h2>
  <slot />
</div>
