<script>
    import Link from "./Link.svelte";

    export let name;
    export let links;
</script>

<li>
    <ul>
        <h4>{name}</h4>
        {#each links as link}
            <Link address={link} />
        {/each}
    </ul>
</li>

<style>

    li {
        display: flex;
        justify-content: center;
    }

    h4 {
        color: var(--white);
        position: absolute;
        writing-mode: vertical-rl;
        -moz-writing-mode: sideways-lr;
        transform: rotate(180deg);
        left: -2rem;
    }

    ul {
        list-style: none;
        border-left: 1px solid var(--white);
        height: max-content;
        padding-left: 1rem;
        position: relative;
        min-height: 5rem;
    }
</style>
    