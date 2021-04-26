<script>
  import { scale,fade,blur } from "svelte/transition";
  import { onMount } from "svelte";

  let toggle = false;

  onMount(() => {
    setInterval(() => {
      toggle = !toggle;
    }, 1500);
  });
</script>
{#if toggle}
	<h3 transition:fade="{{delay: 250, duration: 300}}">
	1哈哈哈哈哈哈哈哈哈哈
	</h3>
{/if}
<div>
  {#if toggle}
    <h1 transition:scale>2哈哈哈哈哈哈哈哈哈哈</h1>
  {/if}
</div>

{#if toggle}
	<h3 transition:blur="{{amount: 10}}">
		3哈哈哈哈哈哈哈哈哈哈
	</h3>
{/if}
