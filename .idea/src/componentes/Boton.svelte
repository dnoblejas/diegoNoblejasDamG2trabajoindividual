<script>
    export let etiqueta = "Hacer clic";
    export let alHacerClic = () => {};
</script>

<button on:click={alHacerClic}>
    {etiqueta}
</button>
