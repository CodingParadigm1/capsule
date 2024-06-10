<script>
	import HistoryCard from './HistoryCard.svelte';
    // 1. documents user activity. 
    // 2. creates temp copy of local databases. 
    // 2 (continued).creates a sandbox for local databases. 
    let current_projects = [
        {
            "title": "test_proj", 
            "db": "MongoDB", 
            "tables": 8
        }
    ]; 
</script>

<main>
    <h1>
        History
    </h1>
    <ul>
        {#each current_projects as projs}
            <HistoryCard/>
        {/each}
    </ul>
</main>

<style>
    main{
        padding:15px 5px;
        background-color: rgb(31, 30, 30);
        display: flex;
        flex-direction: column;
        justify-content: start;
        align-items: center;

    }
    ul{
        width:400px;
    }
</style>
