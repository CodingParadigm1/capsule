<script>
    // 1. documents user activity. 
    // 2. creates temp copy of local databases. 
    // 2 (continued).creates a sandbox for local databases. 
    let current_projects = []; 
</script>

<h1>
    History
</h1>

{#each current_projects as projs}
     {
        projs
     }
{/each}