<script>
let typebadge;
let mdp1 ='';
let mdp2 ='';


</script>

<div class="mx-auto flex min-h-screen w-full items-center justify-center bg-gray-900 text-white">
  <section class="flex w-[30rem] flex-col space-y-10">
      <div class="text-center text-4xl font-medium">Creez un compte</div>
       <div
        class="w-full transform border-b-2 bg-transparent text-lg duration-300 focus-within:border-indigo-500"
      >
        <input 
          type="text"
          placeholder="Pseudo"
          class="w-full border-none bg-transparent outline-none placeholder:italic focus:outline-none"
        />
      </div>

      <div
        class="w-full transform border-b-2 bg-transparent text-lg duration-300 focus-within:border-indigo-500"
      >
        <input
          type="text"
          placeholder="Email"
          class="w-full border-none bg-transparent outline-none placeholder:italic focus:outline-none"
        />
      </div>

      <div
        class="w-full transform border-b-2 bg-transparent text-lg duration-300 focus-within:border-indigo-500"
      >
        <input bind:value={mdp1} 
          type="password"
          placeholder="Mot de passe"
          class="w-full border-none bg-transparent outline-none placeholder:italic focus:outline-none"
        />
      </div>
      <div
        class="w-full transform border-b-2 bg-transparent text-lg duration-300 focus-within:border-indigo-500 inline-block"
      >
         
        <input bind:value={mdp2} 
          type="password"
          placeholder="Confirmez mot de passe" 
          class=" border-none bg-transparent outline-none placeholder:italic focus:outline-none inline-block"
        />
        {#if mdp1 == mdp2 && mdp1.length >= 4}
        <div id="boutonrouge" class="badge badge-success">
          <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="inline-block w-4 h-4 stroke-current" bg-red><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path></svg>
        </div>
        {:else}
        <div id="boutonrouge" class="badge badge-error">
          <svg xmlns="http://www.w3.org/2000/svg"  viewBox="0 0 24 24" fill="none" class="inline-block w-4 h-4 stroke-current" bg-red><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"  d="M406.656 706.944L195.84 496.256a32 32 0 1 0-45.248 45.248l256 256l512-512a32 32 0 0 0-45.248-45.248L406.592 706.944z"></path></svg>
        </div>
        {/if}
      </div>

      <button
        class="transform rounded-sm bg-indigo-600 py-2 font-bold duration-300 hover:bg-indigo-400"
      >
       Creer un compte 
      </button>

      <a
        href="#"
        class="transform text-center font-semibold text-gray-500 duration-300 hover:text-gray-300"
        >Mot de passe oublié ?</a
      >

      <p class="text-center text-lg">
        Déjà un compte ?
        <a
          href="#/connexion"
          class="font-medium text-indigo-500 underline-offset-4 hover:underline"
          >Se connecter </a
        >
      </p>
    </section>
  </div>

  <style>
  #boutonrouge{
  display: inline-block;
  float: right;
  }
  </style>