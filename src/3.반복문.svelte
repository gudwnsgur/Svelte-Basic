<script>
	let name = 'Fruits';
	let fruits = ['apple', 'Banana', 'Orange', 'Cherry', "Mango"]
	function deleteFruit() {
		fruits = fruits.slice(1,3);
	}
</script>

<h1>Hello {name}!</h1>


<ul>
	{#each fruits as fruit}
		<li> {fruit} </li>
	{/each}	
</ul>

<ul>
	{#each [...fruits].reverse() as fruit}
	<li> {fruit} </li>
	{/each}
</ul>

<button on:click={deleteFruit}>
	Eat it!
</button>