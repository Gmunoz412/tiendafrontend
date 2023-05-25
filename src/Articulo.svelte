<script>
  export let articulo = {};
</script>

<div class="card">
  <input bind:value={articulo.nombre} class="title" />
  <input
    type="number"
    min="0"
    max="9999.99"
    step=".01"
    bind:value={articulo.precio} />  €
  <slot />
</div>

<style>
   /* Aquí el código CSS */
  /* Consultar el código fuente */
</style>
