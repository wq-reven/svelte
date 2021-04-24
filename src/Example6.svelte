<script>
	import { onMount, beforeUpdate, afterUpdate, onDestroy, tick } from "svelte";
	export let number
	onMount(() => {
		console.log("mounted子组件");
	});
	// beforeUpdate(() => {
	// 	console.log("beforeUpdate");
	// });
	afterUpdate(() => {
		console.log("afterUpdate");
	});
    onDestroy(() => {
        console.log('destroy')
    })
    beforeUpdate(async () => {
		console.log('the component is about to update');
		await tick();
		console.log('the component just updated');
	});
</script>

<div>
    {number}
</div>
// 生命周期
//首次回调运行在onMount初始化之前。

