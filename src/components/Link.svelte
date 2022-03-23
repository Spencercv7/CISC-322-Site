<script>
    export let address;
</script>

<li>
    <a href={address} target="_blank"><p>{address}</p></a>
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

    li {
        position: relative;
        overflow: hidden;
    }

    a:before {
        content: "";
        height: 100%;
        width: 100%;
        background-color: var(--white);
        position: absolute;
        opacity: .2;
        transform: translateX(-100%);
        transition: all .2s;
    }
    
    a:hover:before {
        transform: translateX(0rem);
    }
    
</style>