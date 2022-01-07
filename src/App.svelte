<script>
	let count=0;
	function increment(){
		count+=1;


	}
	function decrement(){
		count-=1

	}
</script>

<main>
	<h1>Hello {name}!</h1>
</main>



<div>Count:{count}</div>
{#if count<5}
<button on:click={increment}>Increment</button>
{:else}
<p>cannot increment</p>
{/if}
<button on:click={decrement}>Decrement</button>