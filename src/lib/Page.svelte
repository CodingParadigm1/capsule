<script>
	import ProjectCard from './ProjectCard.svelte';

</script>

<article>
  <section class="selections">
    <!-- 
      create an each block. refer to inventory page. 
     -->
    <ProjectCard/>
    <ProjectCard/>
    <ProjectCard/>
    <ProjectCard/>
  </section>
  <section class="selections">

  </section>
</article>

<style>
  *{
    color:white;
  }

  section.selections{
      display: flex;
      flex-direction: row;
      align-items: center;
      justify-content: space-around;
      gap: 25px;
  }
</style>