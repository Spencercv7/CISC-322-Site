<script>
    import Section from "./Section.svelte";
    import TeamTile from "./TeamTile.svelte";

    // @ts-ignore
    import { team } from "../data/team.json";
</script>

<Section title={"Team"}>
    {#each team as member}
        <TeamTile data={member} />
    {/each}
</Section>