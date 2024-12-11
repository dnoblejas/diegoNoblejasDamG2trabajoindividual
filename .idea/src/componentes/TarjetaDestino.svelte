<script>
    export let destino = {};
</script>

<div>
    <img src={destino.imagen} alt={destino.nombre} />
    <h3>{destino.nombre}</h3>
    <p>{destino.pais}</p>
    <p>{destino.precio}</p>
</div>
