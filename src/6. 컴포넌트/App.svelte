<script>
	import Fruits from './Fruits.svelte';
	import Hello from './Hello.svelte'
	let fruits = ['Apple', 'Banana', 'Orange', 'Mango', 'Cherry'];
</script>


<Fruits fruitsFromFruits={fruits}/>
<Fruits fruitsFromFruits={fruits} reverse={true}/>
<Fruits fruitsFromFruits={fruits} slice="-2"/>
<Fruits fruitsFromFruits={fruits} slice="0, 3"/>

<Hello />
