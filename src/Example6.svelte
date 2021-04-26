<script>
	import { onMount, beforeUpdate, afterUpdate, onDestroy, tick } from "svelte";
	export let number
  let text = `Select some text and hit the tab key to toggle uppercase`;
    onMount(() => {
      console.log("mounted子组件");
    });

    afterUpdate(() => {
      console.log("afterUpdate");
    });
    beforeUpdate(async () => {
      //首次回调运行在onMount初始化之前。
      console.log('the component is about to update');
      // await tick();
      console.log('the component just updated');
	  });
</script>

<style>
</style>

<div>
  {number}
</div>



