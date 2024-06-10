<script>
    export let proj_title = "default title", 
               db_name = "MongoDB", 
               quantity = "5"; 
</script>


<main>
    <h2>
        {proj_title}
    </h2>

    <section>
        <span>
            {db_name}
        </span>
        <span>
            {quantity} <!-- Lists the number of tables in project-->
        </span>
    </section>
</main>

<style>
    main{
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        width:100px;
        height:45px;
        background-color: black;
    }
</style>