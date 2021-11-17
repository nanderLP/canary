<script>
  import BaseExperiment from "./BaseExperiment.svelte";
</script>

<BaseExperiment
  title="color-scheme"
  mdnLink="https://developer.mozilla.org/en-US/docs/Web/CSS/color-scheme"
>
  <p>
    This website is using <code>color-scheme</code> right now! Basic variables like
    the background and text color were changed based on your theme preference without
    any further configuration.
  </p>
  <pre>
      <code>
    <meta name="color-scheme" content="dark light" />
</code></pre></BaseExperiment
>

<style>
  div {
    color-scheme: light;
  }
</style>
