<script>
	import Output from "./Output.svelte";
	export let goal = "be number 1";
</script>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}
</style>

<main>
	Write your goal!
	<input type="text" bind:value={goal} />
	<Output userGoal={goal} />
</main>
