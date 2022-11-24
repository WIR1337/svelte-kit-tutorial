<script>
let count = 0;


</script>
<h1>Welcome to SvelteKit</h1>

<a href="/about">About</a>
<a href="/parameters">Parameters</a>
<div>Счетчик = {count}</div>
<button on:click={() => {count += 1}}>+</button>
<button on:click={() => {count -= 1}}>-</button>