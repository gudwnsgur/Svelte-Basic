<script>
	// props
	export let fruitsFromFruits;
	export let reverse;
	export let slice;
	
	let computedFruits = [];
	let name = '';
	
	if(reverse) {
		computedFruits = [...fruitsFromFruits].reverse();
		name = 'reverse';
	}
	else if(slice){
		computedFruits = fruitsFromFruits.slice(...slice.split(','))
		// name = "slice " + slice
		name = `slice ${slice}`
	}
	else {
		computedFruits = fruitsFromFruits
	}
</script>





<h2> Fruits {name} </h2>
<ul>
	{#each computedFruits as fruit}
	<li> {fruit} </li>
	{/each}
</ul>

