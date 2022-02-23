<script>

    export let data;

</script>

<li>
    <p>{data.title}</p>
    <a href={`/${data.pdf}`}>View Document</a>
</li>

<style>

    li {
        height: 20rem;
        width: 20rem;
        background-color: var(--white);
        border-radius: 2%;
        position: relative;
        transition: all .1s;
    }

    li:hover {
        form: scale(1.01)
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