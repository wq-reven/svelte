<script>
  let count = 0
</script>

 <p>clicked {count} times</p>
<button on:click={() =>{ count ++ }}>
  Click
</button>


<!-- import React, { useState } from 'react';

function Example() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click
      </button>
    </div>
  );
} -->