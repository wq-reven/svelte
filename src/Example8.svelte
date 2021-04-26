<script>
  import { draw } from "svelte/transition";
  import { onMount } from "svelte";
  import { quintOut } from 'svelte/easing';

  let toggle = false;

  onMount(() => {
    setInterval(() => {
      toggle = !toggle;
    }, 5000);
  });
</script>


<svg viewBox="0 0 5 5" xmlns="http://www.w3.org/2000/svg">
	{#if toggle}
		<path transition:draw="{{duration: 3500, delay: 0, easing: quintOut}}"
					d="M2 1 h1 v1 h1 v1 h-1 v1 h-1 v-1 h-1 v-1 h1 z"
					fill="none"
					stroke="cornflowerblue"
					stroke-width="0.1px"
					stroke-linejoin="round"
		/>
	{/if}
</svg>