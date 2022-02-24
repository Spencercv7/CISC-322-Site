<script>

    export let data;

</script>

<li>
    <span>{data.title ? data.title : "Coming Soon..."}</span>
    {#if data.title !== ""}
        <div>
            <a href={`/pdf/${data.pdf}`} target="_blank">
                <p>View PDF</p>
            </a>
            <a href={data.videoURL} target="_blank">
                <p>View Video</p>
            </a>
        </div>
        <img src={`/img/${data.img}`} alt={data.title}/>
    {/if}
</li>

<style>

    li {
        background-color: var(--white);
        position: relative;
        transition: all .1s;
        aspect-ratio: 8.5 / 11 ;
        height: 25rem;
        transition: all .2s;
        cursor: pointer;
        overflow: hidden;
    }

    li:hover div {
        transform: translateX(0rem);
    }

    li:hover span {
        transform: translateX(100%);
    }

    div {
        background-color: var(--accent);
        opacity: .95;
        height: 100%;
        width: 100%;
        position: absolute;
        transform: translateX(-100%);
        transition: all .2s;

        display: grid;
        grid-template-rows: repeat(2, 1fr);
    }


    a {
        place-self: center;
        appearance: none;
        text-decoration: none;
        transition: all .2s;
    }

    a:hover {
        transform: scale(1.05);
    }

    a p {
        color: var(--white);
        background-color: var(--black);
        padding: 1rem;
    }

    span {
        background-color: var(--accent);
        color: var(--white);
        position: absolute;
        bottom: 0;
        right: 0;
        padding: .2rem;
        transition: all .2s;
    }

    img {
        height: 100%;
        width: 100%;
        object-fit: cover;
    }

</style>