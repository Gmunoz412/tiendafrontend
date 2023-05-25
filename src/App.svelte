<script>
  import { Router } from "svelte-routing";
  import Nav        from "./Nav.svelte";
  import Contenido  from "./Contenido.svelte";

  import { setContext } from "svelte";
	
  const urlArticulos = "https://tiendabackend.herokuapp.com/api/articulos/";

  setContext("urlArticulos", urlArticulos);

</script>

<Router>
  <Nav />
  <Contenido />
</Router>

<style>
  @import url("https://fonts.googleapis.com/css?family=Aclonica");

  :global(*) {
    margin: 0;
    padding: 0;
  }

  :global(body) {
    display: flex;
    flex-direction: column;
    font-family: "Aclonica";
  }
 
  :global(a:hover) {
    text-decoration: none;
    cursor: pointer;
  }
</style>
