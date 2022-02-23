<script>
    import AssignmentCard from './AssignmentCard.svelte'
    import Section from './Section.svelte';
    import {assignemnts} from '../data/assignments'
</script>

<Section title={"Assignments"}>
    {#each assignments as assignment}
        <AssignmentCard data={assignment} />
    {/each}
</Section>