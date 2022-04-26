<script>
	import products from '$lib/listing.js'
	let name = 'Romain'
</script>

<section>
	<h1>Listing produits</h1>
	{#each products as product}
		<div class="card">{product.name}</div>
	{/each}
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	.card {
		border: solid 1px black;
		width: 80%;
		margin: 10px;
		padding: 20px;
	}
</style>
