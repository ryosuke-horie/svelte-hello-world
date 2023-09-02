<script>
	let name = 'Svelte';

    // カウントボタン
	let count = 0;

	function increment() {
		count += 1;
	}

    // リアクティブ宣言
 	$: doubled = count * 2;
</script>

<h1>Hello {name.toUpperCase()}!</h1>


<p>This is a paragraph.</p>

<button on:click={increment}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>

<p>{count} doubled is {doubled}</p>


<style>
	p {
		color: goldenrod;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>

