<script>
	let name = 'Svelte';

    // カウントボタン
	let count = 0;

	function increment() {
		count += 1;
	}
</script>

<h1>Hello {name.toUpperCase()}!</h1>


<p>This is a paragraph.</p>

<button on:click={increment}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>


<style>
	p {
		color: goldenrod;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>

