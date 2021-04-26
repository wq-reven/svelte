<script>
    import { count } from './store';
  function increment() {
        $count += 1;
    }
</script>
<button on:click={increment}>增加</button>