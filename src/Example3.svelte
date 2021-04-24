<script>
    import App from './App.svelte'
import Example4 from './Example4.svelte'
    let data = {
       name:'svelte',
       address:'https://www.sveltejs.cn/'
    }
</script>

<div class=''>
    <Example4 data={data} {...data}  />
</div>