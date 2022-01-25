<script>
    import Link from "./Link.svelte";

    export let name;
    export let links;
</script>

<div>
    <ul>
        <h3>{name}</h3>
        {#each links as link}
            <Link address={link} />
        {/each}
    </ul>
</div>

<style>

    div {
        display: flex;
        justify-content: center;
    }

    h3 {
        color: var(--white);
        position: absolute;
        writing-mode: sideways-lr;
        text-orientation: mixed;
        left: -2rem;
    }

    ul {
        list-style: none;
        border-left: 1px solid var(--white);
        height: max-content;
        padding-left: 1rem;
        position: relative;
    }
</style>
    