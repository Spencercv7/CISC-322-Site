<script>
    export let address;
</script>

<li>
    <a href={address}><p>{address}</p></a>
</li>

<style>
    a, a:visited, a:active{
        color: var(--accent);
    }

    p {
        text-overflow: ellipsis;
        white-space: nowrap;
        width: 250px;
        overflow: hidden;
    }
</style>