<script>
	import Bag from '../../components/bag.svelte';
	import { bags } from '../../bags-store';
</script>

<div class="bags container">
	{#each $bags as bag}
		<Bag description={bag.description} price={bag.price} img={bag.Image} />
	{/each}
</div>
<!-- <div class="bags">
	<Bag description={$bags[1].description} price={$bags[1].price} img={$bags[1].Image} />
	<Bag description={$bags[2].description} price={$bags[2].price} img={$bags[2].Image} />
	<Bag description={$bags[11].description} price={$bags[11].price} img={$bags[11].Image} />
    <Bag img="../../src/bags-imgs/IMG-20210823-WA0002.jpg" />
</div> -->
<style>
	.bags {
		display: grid;
		/* grid-template-columns: 50% 50%; */
	}
	.container {
		max-width: 460px;
		margin: auto;
		text-align: center;
	}
</style>
