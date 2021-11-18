<script>
  import BaseExperiment from "./BaseExperiment.svelte";
  let color;
  color = "#8f9aff";
</script>

<BaseExperiment
  title="accent-color"
  mdnLink="https://developer.mozilla.org/en-US/docs/Web/CSS/accent-color"
>
  <div style="--color: {color}">
    <p>
      An amazing CSS property which styles some form elements based on the
      provided color! Pick one and see how the elements change.
    </p>
    <input class="my-2" type="color" bind:value={color} />
    <span>Selected color: {color}</span>
    <fieldset class="flex flex-col children:my-2">
      <span>
        <input type="checkbox" id="checkbox" />
        <label for="checkbox">Epic checkbox</label></span
      >
      <span>
        <input type="radio" id="radioOne" name="owo" />
        <label for="radioOne">Epic radio input</label>
      </span>
      <span
        ><input type="radio" id="radioTwo" name="owo" />
        <label for="radioTwo">Another epic radio input</label>
      </span>
    </fieldset>
  </div></BaseExperiment
>

<style>
  div {
    accent-color: var(--color);
  }
  fieldset input[type="checkbox"],
  fieldset input[type="radio"] {
    transform: scale(2);
    @apply mx-1.5;
  }
</style>
