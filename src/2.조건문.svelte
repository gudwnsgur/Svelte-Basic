<script>
	let name = '형준혁';
	let toggle = false;
</script>

<!-- #, :, / 순서 -->
{#if toggle}  
<h1>
	hello {name}
</h1>
{:else}
<h1>
	 no name!
</h1>
{/if}

<button on:click={()=>
	{toggle = !toggle}}>
button
</button>
