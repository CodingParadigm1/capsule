<script>
	import History from './History.svelte';
    // 1. documents user activity. 
    // 2. creates temp copy of local databases. 
    // 2 (continued).creates a sandbox for local databases. 
    let current_projects = []; 
</script>

<main>
    <h1>
        History
    </h1>
    {#each current_projects as projs}
        {
        projs
        }
    {/each}
</main>

<style>
    main{
        background-color: black;
        display: flex;
        align-items: center;
        justify-content: center;
    }
</style>
