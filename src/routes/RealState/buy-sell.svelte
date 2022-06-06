<script>
	import RealStateCard from '../../components/RealStateCard.svelte';
	import { RealStates } from '../../store';
</script>

<main>
	<h2>real state in rabak</h2>
</main>

{#each $RealStates as land}
	<RealStateCard
		Image={land.Image}
		description={land.description}
		landOwner={land.Image}
		location={land.Image}
	/>
{/each}

<style lang="scss">
	main {
		text-align: center;
	}
</style>
