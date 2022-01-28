<script>
    import Section from "./Section.svelte"
    import LinkList from "./LinkList.svelte";

    // Data import.
    import {core, general, video} from "../data/links.json";
</script>

<Section title={"Links"}>
    <LinkList name={"core"} links={core} />
    <LinkList name={"general"} links={general}/>
    <LinkList name={"videos"} links={video}/>
</Section>