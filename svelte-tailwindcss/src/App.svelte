<script>
  import svelteLogo from './assets/svelte.svg'
  import tailwindcssLogo from './assets/tailwindcss.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
</script>

<main>
  <div class="container mx-auto">
    <div class="flex justify-center">
      <a href="https://vitejs.dev" target="_blank" rel="noreferrer">
        <img src={viteLogo} class="logo" alt="Vite Logo" />
      </a>
      <a href="https://svelte.dev" target="_blank" rel="noreferrer">
        <img src={svelteLogo} class="logo svelte" alt="Svelte Logo" />
      </a>
      <a href="https://tailwindcss.com" target="_blank" rel="noreferrer">
        <img src={tailwindcssLogo} class="logo" alt="Tailwind CSS Logo" />
      </a>
    </div>
    <h1 class="text-center text-3xl font-bold text-blue-500">Vite + Svelte + tailwindcss</h1>

    <div class="mx-auto flex justify-center mt-6">
      <Counter />
    </div>
    <div class="flex justify-center flex-col items-center mt-6">
      <p>
        Check out <a href="https://github.com/sveltejs/kit#readme" target="_blank" rel="noreferrer">SvelteKit</a>, the official Svelte app framework powered by Vite!
      </p>

      <p class="read-the-docs">Click on the Vite and Svelte logos to learn more</p>
    </div>
  </div>
</main>

<style>
  .logo {
    height: 6em;
    padding: 1.5em;
    will-change: filter;
    transition: filter 300ms;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.svelte:hover {
    filter: drop-shadow(0 0 2em #ff3e00aa);
  }
  .read-the-docs {
    color: #888;
  }
</style>
