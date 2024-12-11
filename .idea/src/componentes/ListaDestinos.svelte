<script>
    import { destinos } from "../datos/destinos.js";
    import TarjetaDestino from "./TarjetaDestino.svelte";
</script>

<div>
    {#each destinos as destino}
        <TarjetaDestino {destino} />
    {/each}
</div>
