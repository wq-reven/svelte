<script>
	import Example6 from './Example6.svelte'
	import { onMount, beforeUpdate, afterUpdate } from "svelte";
	let number = 1
	onMount(() => {
		console.log("mounted父组件");
	});
</script>

<div>
	<Example6 number={number} />
	<button on:click={() => {
		number ++
	}}>增加number</button>
</div>
// 生命周期
