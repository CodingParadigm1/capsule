<script>
  import Main from './lib/Page.svelte';
  import Menu from './lib/Menu.svelte';
  import Inventory from './lib/Inventory.svelte';
  import History from './lib/History.svelte';
  let pages = [Main, Inventory, History]; 
  let current_page = 0; 
</script>

<main>
  <Menu bind:page_counter={current_page}/>
  <article class:grid-form={current_page>0}>
    {#if current_page>0}
       <section></section>
    {/if}
    <svelte:component this={pages[current_page]}/>
    {#if current_page>0}
        <section></section>
    {/if}
  </article>
</main>

<style>
  main{
    display: flex;
    flex-direction: column;
    align-items: center;
    width:100%;
    height: 100vh; /* Set main height to 100% of viewport height */
  }
  .grid-form{
    display: grid;
    grid-template-columns: 1fr 7fr 1fr; /* Changed grid-template-columns to use fractions */
    width:100%;
    min-width:250px;                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      
    max-width:1050px;
    height: 100%; /* Set article height to 100% of its container (main) */
    flex-grow: 1; /* Allow the article to grow to fill remaining space */
  }
  @media only screen and (max-width:425px){
    .grid-form{
      grid-template-columns: 1fr 12fr 1fr;
    }
  }
</style>