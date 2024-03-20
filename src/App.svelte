<!-- Script JS -->
<script>
    let magnitudes = [10, 25, 50, 100]
</script>

<!-- Estructura contenido HTML -->
<div class="container">
    {#each magnitudes as m}
        <div class="col-wrap">
            <div class = 'column' style='height: {m}px'></div>
            <img class = 'mask' src="./images/tipito.svg" alt="">
        </div>
        
    {/each}
</div>
<!-- Estilos CSS -->
<style>
    .container{
        display: flex;
        align-items: flex-end;
        justify-content:center;
    }
    .column{
        background-color: blue;
        width: 50px;
        /*margin: 10px;*/
        
    }
    .mask{
        width: 50px;
        height:100px;
        position: absolute;
        bottom: 0;
    }
    .col-wrap{
        position: relative;
        border: 1px solid black;
        width: 50px;
        margin: 5px;
    }

</style>
