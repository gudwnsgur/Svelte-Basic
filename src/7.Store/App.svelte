<script>
	import { storeName } from './store.js';
	import Parent from './Parent.svelte';
	
	let name = "world";
	// storeName은 객체이기 때문에 $를 붙여 데이터처럼 사용
	$storeName = name;
</script>

<h1>
	hello {name}!!
</h1>
<Parent/>