<script>
    export let data;
</script>


<li>
    <figure>
        <img src="{data.imageURL}" alt="{data.name}"/>
    </figure>
    <p>{data.name}</p>
</li>

<style>
    li {
        position: relative;
        display: flex;
        gap: 1rem;
        flex-direction: column;
        align-items: center;
        margin-bottom: 2rem;
    }

    img {
        object-fit: cover;
        height: 100%;
        width: 100%;
        background-color: var(--white);
    }

    figure {
        position: relative;
        height: 125px;
        width: 125px;
        overflow: hidden;
        border-radius: 100%;
    }

    p {
        place-self: center;
        color: var(--white);
        font-size: 1.15rem;
    }

</style>