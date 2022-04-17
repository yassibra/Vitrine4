<script>
  import Home from '../src/Home.svelte';
  import Connexion from '../src/Connexion.svelte';
  import NotFound from '../src/NotFound.svelte';
  import Router from 'svelte-spa-router';
  import CreerCompte from '../src/CreerCompte.svelte';

 
</script>

<Router routes={{
  '/connexion': Connexion,
  '/creercompte': CreerCompte,
  '/': Home,
  '*': NotFound
}}
/>
<hr>



