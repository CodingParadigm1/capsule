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
  <svelte:component this={pages[current_page]}/>
</main>

<style>
  main{
    display: flex;
    flex-direction: column;
    align-items: center;
    gap:15px;
  }
</style>