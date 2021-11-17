<script>
  import "virtual:windi.css";
  import AccentColor from "./components/experiments/AccentColor.svelte";
  import ColorScheme from "./components/experiments/ColorScheme.svelte";
</script>

<main class="mx-auto max-w-prose">
  <div class="my-8" id="intro">
    <h1 class="text-3xl">experimental web features</h1>
    <p class="my-2">
      Hey! This is a little website made by
      <a href="https://github.com/nanderLP">nander</a> to explore the latest web
      features.
      <br />
      It's built with <a href="https://vitejs.dev">vite</a>, <a href="https://svelte.dev">svelte</a> and
      <a href="https://windicss.org">windicss</a>.
      <br />
      It's strongly recommended to use an up-to-date chromium-based browser.
    </p>
  </div>
  <div class="grid gap-4" id="playground">
    <ColorScheme />
    <AccentColor />
  </div>
</main>

<style>
  #intro a {
    color: var(--primary);
  }
</style>
