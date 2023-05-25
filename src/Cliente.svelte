<script>
  export let cliente = {};
</script>

<div class="card">
  <input bind:value={cliente.nombre} class="title" />
  <input bind:value={cliente.apellidos} class="title" />
  <slot />
</div>

<style>
  /* Aquí el código CSS */
  /* Consultar el código fuente */
</style>
