<script>
  import Nav from '../src/Nav.svelte';
  import Footer from '../src/Footer.svelte';
  import DivCreerCompte from '../src/DivCreerCompte.svelte';

   const pkg = {
    titresite: 'Telegram Genius'
  };
</script>

<Nav {...pkg} />
<DivCreerCompte/>
<Footer/>