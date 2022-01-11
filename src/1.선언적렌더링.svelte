<script>
	let name = 'world';
	let age = '10';
	
	setTimeout(() => {
		age = 70;
	}, 3000);
	
	function assign() {
		name = "assigned!!";
		age = 3;
	}
</script>

<h1 class = {age < 50 ? 'active' : ''}>Hello {name}!</h1>

<h1>
	my age = {age}
</h1>

<img src="" alt={name} />
<input type="text" bind:value= {name}/>

<button on:click={assign}>
	assign
</button>

<style>
	h1 {
		color : red;
	}
	.active{
		color : blue;
	}
</style>