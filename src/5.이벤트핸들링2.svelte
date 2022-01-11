<script>
	let text = 'abdb'
</script>

<h1>
	{text}
</h1>
<!-- <input type="text" 
			 value = "{text}"  script -> html
			 on:input={(e) => { text = e.target.value }} html -> script
/>  
-->

<!-- 양방향 바인딩 -->
<input type="text"
			 bind:value = {text}/>


<button on:click={()=> {text = 'heo'}}>
	click
</button>
