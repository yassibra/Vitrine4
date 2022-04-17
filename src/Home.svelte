<script>
  import { onMount } from 'svelte';
  import Nav from '../src/Nav.svelte';
  import Footer from '../src/Footer.svelte';
  import Section from '../src/Section.svelte';
  import NotFound from '../src/NotFound.svelte';
  import Connexion from '../src/Connexion.svelte';
  import {push, pop, replace} from "svelte-spa-router";
  let photos = [];

	onMount(async () => {
		const res = await fetch(`http://78.199.207.79.localhost:8000/users/`);
		photos = await res.json();
    console.log(photos)
	});
   const pkg = {
    titresite: 'Telegram Genius'
  };
</script>
<Nav {...pkg} />
<Section/>
<Footer/>
{#each photos as photo}
	<p>{photo.test}</p>
{/each}
<p>WSH</p>

