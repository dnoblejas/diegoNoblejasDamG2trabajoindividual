<script>
    let items = [
        { id: 1, title: 'Elemento 1', description: 'Descripción del primer elemento' },
        { id: 2, title: 'Elemento 2', description: 'Descripción del segundo elemento' },
        { id: 3, title: 'Elemento 3', description: 'Descripción del tercer elemento' }
    ];

    function mostrarDetalle(id) {
        alert(`Detalles de: ${id}`);
    }
</script>

<main>
    <h1>Lista de Elementos</h1>

    <div class="container">
        {#each items as item (item.id)}
            <div class="card">
                <h2>{item.title}</h2>
                <p>{item.description}</p>
                <button on:click={() => mostrarDetalle(item.id)}>Ver Detalles</button>
            </div>
        {/each}
    </div>
</main>

<style>
    main {
        font-family: Arial, sans-serif;
        text-align: center;
        padding: 20px;
    }

    h1 {
        color: #4CAF50;
    }

    .container {
        display: flex;
        justify-content: space-around;
        flex-wrap: wrap;
        margin-top: 20px;
    }

    .card {
        background-color: #f4f4f4;
        padding: 20px;
        margin: 10px;
        width: 200px;
        border-radius: 8px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        text-align: left;
    }

    .card h2 {
        font-size: 18px;
        color: #333;
    }

    .card p {
        font-size: 14px;
        color: #777;
    }

    button {
        background-color: #4CAF50;
        color: white;
        border: none;
        padding: 8px 16px;
        border-radius: 4px;
        cursor: pointer;
    }

    button:hover {
        background-color: #45a049;
    }
</style>
