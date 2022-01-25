<script>
    import Section from "./Section.svelte"
    import LinkList from "./LinkList.svelte";

    // Data import.
    import {core, general, video} from "../data/links.json";
</script>

<Section title={"Links"}>
    <div>
        <LinkList name={"core"} links={core} />
        <LinkList name={"general"} links={general}/>
        <LinkList name={"videos"} links={video}/>
    </div>
</Section>

<style>
    div {
        width: 100%;
        
        display: grid;
        grid-template-columns: repeat(3, 1fr);

        gap: 1rem;

        position: relative;
    }

    @media only screen and (max-width: 1100px) {
        div {
            grid-template-columns: 1fr
        }
    }
</style>