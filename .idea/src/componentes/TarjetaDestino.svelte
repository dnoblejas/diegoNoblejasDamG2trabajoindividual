<script>
    export let destino = {
        id: 0,
        nombre: "",
        pais: "",
        precio: "",
        imagen: ""
    };
</script>

<div class="destino">
    <img src={destino.imagen} alt={destino.nombre} />
    <h3>{destino.nombre}</h3>
    <p>{destino.pais}</p>
    <p>{destino.precio}</p>
</div>

<style>
    .destino {
        margin-bottom: 1rem;
        border: 1px solid #ccc;
        padding: 1rem;
        border-radius: 8px;
    }
    .destino img {
        max-width: 100%;
        border-radius: 8px;
    }
    .destino h3 {
        margin-top: 0.5rem;
    }
    .destino p {
        margin: 0.25rem 0;
    }
</style>
