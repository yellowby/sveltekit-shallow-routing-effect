<script>
  import {pushState} from "$app/navigation";

  let { url, children } = $props();

  function onclick() {
    pushState(url, {})
  }
</script>

{#if children}
  <button {onclick}>
    {@render children()}
  </button>
{/if}
