<!-- Script JS -->
<script>
    let magnitudes = [10, 25, 50, 100]
</script>

<!-- Estructura contenido HTML -->
<h1 class="titulo">Representación de distintas magnitudes en el consumo de agua de una persona</h1>
<div class="col-container">
    {#each magnitudes as m}
        <div class="col-wrap">
            <div class = 'column' style='height: {m*2}px'></div>
            <img class = 'mask' src="./images/tipito.svg" alt="">
        </div>
        
    {/each}
</div>


<!-- Estilos CSS -->
<style>
    .titulo{
        font-family: 'Times New Roman', Times, serif;
        font-weight: bold;
        text-decoration: underline;
        text-align: center;
    }
    .col-container{
        
        display: flex;
        align-items: flex-end;
        justify-content:center;
    }
    .column{
        background-color: blue;
        /*background-image: './images/agua.jpg';*/
        width: 100px;
        
    }
    .mask{
        width: 100px;
        height:200px; /*sale columna por abajo xq el svg tiene parte por abajo de borde de figura*/
        position: absolute;
        bottom: 0;
        z-index: 1;
    }
    .col-wrap{
        position: relative;
        width: 100px;
        margin: 10px;
    }


</style>
