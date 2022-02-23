<script>

    export let data;

</script>

<li>
    <p>{data.title ? data.title : "Coming Soon..."}</p>
   
    {#if data.title !== ""}
        <a href={`/pdf/${data.pdf}`} target="_blank">View Document</a>
        <a href={`${data.videoURL}`} target="_blank">View Video</a>
    {/if}
</li>

<style>

    li {
        height: 20rem;
        width: 20rem;
        background-color: var(--white);
        border-radius: 2%;
        position: relative;
        transition: all .1s;

        display: grid;
        grid-template-rows: repeat(2, 1fr);
    }

    li:hover {
        form: scale(1.01)
    }

    a {
        place-self: center;
    }

    p {
        background-color: var(--accent);
        color: var(--white);
        position: absolute;
        bottom: 0;
        right: 0;
        padding: .2rem;
    }

</style>