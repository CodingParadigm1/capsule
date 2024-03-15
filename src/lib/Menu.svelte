<script>
    export let page_counter = 0; 
    import menuCss from "./menu.module.css";
</script>
 

<nav class="nav">
<!-- 
    method BEM (Block - Element - Modify)
 -->
    <ul class="list">
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
      <li class="list__title" on:click={()=>page_counter = 0}>Workflow</li>
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
      <li class="list__title" on:click={()=>page_counter=1}>Inventory</li>
      <!-- svelte-ignore a11y-click-events-have-key-events -->
      <!-- svelte-ignore a11y-no-noninteractive-element-interactions -->
      <li class="list__title--white" on:click={()=>page_counter=2}>History</li>
    </ul>
</nav>

  
