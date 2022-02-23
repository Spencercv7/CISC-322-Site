<script>
    import AssignmentCard from './AssignmentCard.svelte'
    import Section from './Section.svelte';
    import {assignments} from '../data/assignments'
</script>

<Section title={"Assignments"}>
    {#each assignments as assignment}
        <AssignmentCard data={assignment} />
    {/each}
</Section>