<script>
  export let title;
  export let mdnLink;
</script>

<div>
  <h2 class="text-xl"><code>{title}</code></h2>
  <a href={mdnLink}>view on mdn</a>
  <slot />
</div>

<style>
  a {
    color: var(--subtitle);
  }
</style>
