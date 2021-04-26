<script>
  let count = 1

  // 反应式声明
  // $:double = count * 2
  // $:console.log(`count:${count}`)
  // $:console.log(`count:${double}`)
  // $:if(count > 5){
  //   alert(count)
  // }

  // let numbers = [1,2,3,4]
  // function addNum(){
  //   numbers.push(numbers.length + 1)
  //   // numbers = numbers
  // }
  // $: numbersStr = numbers.join(',')
</script>


 <p>clicked {count} times</p>
<button on:click={() =>{ count ++ }}>
  Click
</button>

<!-- {#if count > 5 }
	<p>count > 5</p>
{/if} -->

<!-- <p>double: {double}</p> -->


<!-- <p>{numbersStr}</p>
<button on:click={addNum}> add number </button> -->