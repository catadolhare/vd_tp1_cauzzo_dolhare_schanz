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
        /*background-image: './images/agua.jpg';*/
        width: 50px;
        
    }
    .mask{
        width: 50px;
        height:100px; /*sale columna por abajo xq el svg tiene parte por abajo de borde de figura*/
        position: absolute;
        bottom: 0;
        z-index: 1;
    }
    .col-wrap{
        position: relative;
        width: 50px;
        margin: 5px;
    }


</style>
