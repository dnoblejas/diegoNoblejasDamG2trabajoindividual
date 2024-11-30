<script>
    export let items = [];
</script>

<nav>
    {#each items as item}
        <a href="#">{item}</a>
    {/each}
</nav>

<style>
    nav {
        display: flex;
        justify-content: space-between;
        background-color: green;
        padding: 1rem;
        color: white;
    }
    a {
        color: white;
        text-decoration: none;
        margin: 0 1rem;
    }
</style>
