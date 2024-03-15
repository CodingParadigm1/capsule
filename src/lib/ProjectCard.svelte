<script>
    export let title = "default", db_size=0, address="0.0.0.0:1234"; 
</script>

<article>
    <h2>
        {title}
    </h2>
    <section id="details">
        <span>
            {db_size}
        </span>
        <span>
            {address}
        </span>
    </section>
</article>

<style>
    *{
        color:white;
    }

    article{
        background-color: rgb(44, 44, 44);
        height:275px;
        width:175px;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: space-around;
        transition-duration: .75s;
    }
    article:hover{
        background-color: rgb(34, 34, 34);
        box-shadow: 0 0 12px white;
        margin:0 -2px;
    }
    article:active span, article:active h2{
        transition-duration: 0s;
        color:grey;
    }
    section#details{
        display: flex;
        flex-direction: column;
        gap:10px;
    }
</style>