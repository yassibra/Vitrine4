<script>
  import Nav from '../src/Nav.svelte';
  import Footer from '../src/Footer.svelte';
  import Section from '../src/Section.svelte';
  import NotFound from '../src/NotFound.svelte';
  import Connexion from '../src/Connexion.svelte';
  import DivConnexion from '../src/DivConnexion.svelte';

   const pkg = {
    titresite: 'Telegram Genius'
  };
</script>

<Nav {...pkg} />
<DivConnexion/>
<Footer/>