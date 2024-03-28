<script>
	let count = 0;
	let obj = {
		count: 0
	}

	function increment() {
		// UPDATING STATE HAPPENS WHEN: 
		// 1. assignment
		// count = 10
		// 2. update statements
		// count++
		// count += 2
		// 3. updating/ assigning a property
		// obj.count++
	
		// UPDATING STATE DOESN'T HAPPENS WHEN: 
		// 1. not an update to svelte
		// data = obj;
		// obj.count++;
		// obj.foo = 1;
		// calling a method
		// obj.push(1)
		count++
	}

	function decrement() {
		count--
	}

	function reset() {
		count = 0;
	}
</script>
<button on:click={decrement}>
	-
</button>

{count}
{JSON.stringify(obj)}

<button on:click={increment}>
	+
</button>
<br />
<button class='reset-btn' on:click={reset}>
	reset
</button>

<style>
	button {
		cursor: pointer;
	}
	.reset-btn {
		width: 63px;
	}
</style>
