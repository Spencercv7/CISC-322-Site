<script>
    import AssignmentCard from './AssignmentCard.svelte'
    import Section from './Section.svelte';
</script>

<Section title={"Assignments"}>
    <ul>
        <AssignmentCard />
        <AssignmentCard />
        <AssignmentCard />
    </ul>
</Section>

<style>
    ul {
        list-style: none;
        width: 100%;
        
        display: grid;
        grid-template-columns: repeat(3, 1fr);

        gap: 1rem;

        position: relative;
    }

    @media only screen and (max-width: 1100px) {
        ul {
            grid-template-columns: 1fr
        }
    }
</style>