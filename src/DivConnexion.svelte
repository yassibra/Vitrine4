<script>
import {push, pop, replace} from "svelte-spa-router";
let mdp = "test";
let email ="test";
const go_connexion = async () => {
  const submit = await fetch("/api", {
    method: "POST",
    body: JSON.stringify({
      email,
      mdp,
    }),
  });
  //push("/creercompte");
}

</script>
<form on:submit|preventDefault={go_connexion}>
<div class="mx-auto flex min-h-screen w-full items-center justify-center bg-gray-900 text-white">
  <section class="flex w-[30rem] flex-col space-y-10">
      <div class="text-center text-4xl font-medium">Connectez-vous</div>

      <div
        class="w-full transform border-b-2 bg-transparent text-lg duration-300 focus-within:border-indigo-500"
      >
        <input bind:value={email}
          type="text"
          placeholder="Email"
          class="w-full border-none bg-transparent outline-none placeholder:italic focus:outline-none"
        />
      </div>

      <div
        class="w-full transform border-b-2 bg-transparent text-lg duration-300 focus-within:border-indigo-500"
      >
        <input bind:value={mdp}
          type="password"
          placeholder="Mot de passe"
          class="w-full border-none bg-transparent outline-none placeholder:italic focus:outline-none"
        />
      </div>

      <button on:click={go_connexion}
        class="transform rounded-sm bg-indigo-600 py-2 font-bold duration-300 hover:bg-indigo-400"
      >
        Se connecter
      </button>

      <a
        href="#"
        class="transform text-center font-semibold text-gray-500 duration-300 hover:text-gray-300"
        >Mot de passe oublié ?</a
      >

      <p class="text-center text-lg">
        Pas de compte ?
        <a
          href="#/creercompte"
          class="font-medium text-indigo-500 underline-offset-4 hover:underline"
          >Creez en un</a
        >
      </p>
    </section>
  </div>
</form>