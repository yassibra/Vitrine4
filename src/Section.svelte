<!-- This example requires Tailwind CSS v2.0+ -->
<script>
import {push, pop, replace} from "svelte-spa-router";
const go_connexion = () => {
  push("#/connexion");
}
</script>
<div class="py-12 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="lg:text-center">
      <h2 id='h2telegram' class="text-base text-indigo-600 font-semibold tracking-wide uppercase color: 0088cc.">Bot Telegram</h2>
      <p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">Le  moyen le plus simple de creer un bot Telegram</p>
      <p class="mt-4 max-w-2xl text-xl text-gray-500 lg:mx-auto"> Avec TelegramGenius, créer un bot Telegram n'a jamais été aussi facile.  </p>
    </div>

    <div class="mt-10">
      <dl class="space-y-10 md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10">
        <div class="relative">
          <dt>
            <div class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white carretelegram">
              <!-- Heroicon name: outline/globe-alt -->
              
              <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
                <path stroke-linecap="round" stroke-linejoin="round" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-16l2.286 6.857L21 12l-5.714 2.143L13 21l-2.286-6.857L5 12l5.714-2.143L13 3z" />
              </svg>
            </div>
            <p class="ml-16 text-lg leading-6 font-medium text-gray-900">Simplissime</p>
          </dt>
          <dd class="mt-2 ml-16 text-base text-gray-500">Telegram Genius propose une interface simple d'utilisation. Il n'est maintenant plus nécessaire d'être developpeur pour créer un bot Telegram. </dd>
        </div>

        <div class="relative">
          <dt>
            <div class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white carretelegram">
              <!-- Heroicon name: outline/scale -->
             <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5" viewBox="0 0 20 20" fill="currentColor">
              <path fill-rule="evenodd" d="M12.395 2.553a1 1 0 00-1.45-.385c-.345.23-.614.558-.822.88-.214.33-.403.713-.57 1.116-.334.804-.614 1.768-.84 2.734a31.365 31.365 0 00-.613 3.58 2.64 2.64 0 01-.945-1.067c-.328-.68-.398-1.534-.398-2.654A1 1 0 005.05 6.05 6.981 6.981 0 003 11a7 7 0 1011.95-4.95c-.592-.591-.98-.985-1.348-1.467-.363-.476-.724-1.063-1.207-2.03zM12.12 15.12A3 3 0 017 13s.879.5 2.5.5c0-1 .5-4 1.25-4.5.5 1 .786 1.293 1.371 1.879A2.99 2.99 0 0113 13a2.99 2.99 0 01-.879 2.121z" clip-rule="evenodd" />
            </svg>
            </div>
            <p class="ml-16 text-lg leading-6 font-medium text-gray-900">Genialissime</p>
          </dt>
          <dd class="mt-2 ml-16 text-base text-gray-500">Pré-visualisez en direct les fonctionnalités que vous voulez apporter à votre Bot. Créer un bot Telegram n'a jamais été autant un plaisir.</dd>
        </div>

        <div class="relative">
          <dt>
            <div class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white carretelegram">
              <!-- Heroicon name: outline/lightning-bolt -->
              <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
              </svg>
            </div>
            <p class="ml-16 text-lg leading-6 font-medium text-gray-900">Une réactivité sans équivalence</p>
          </dt>
          <dd class="mt-2 ml-16 text-base text-gray-500">Votre bot fournira des réponses instannées. Après la confirmation des changements à réaliser, TelegramGenius s'engage à mettre à jour votre bot en 1h.   </dd>
        </div>

        <div class="relative">
          <dt>
            <div class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white carretelegram">
              <!-- Heroicon name: outline/annotation -->
              <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" />
              </svg>
            </div>
            <p class="ml-16 text-lg leading-6 font-medium text-gray-900">Chatbot Intelligent</p>
          </dt>
          <dd class="mt-2 ml-16 text-base text-gray-500">Impressionnez votre communauté avec une fonctionnalité Telegramesque !</dd>
        </div>
      </dl>
    </div>
    <button on:click={go_connexion} id="demarrerbouton" class="lg:px-8 btn bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 carretelegram rounded-full display-flex">
  Démarrer
</button>
  </div>
  

</div>
<div >

</div>

<style>
svg{
  color: #FFFFFF
}
.carretelegram{
  background-color: #0088CC
}
#h2telegram{
  color: #0088CC
}
#demarrerbouton{
  display: block;
  margin: auto;
  margin-top: auto;
}
</style>
