<script>
  export let result;
  export let userGoal;
 
    
    $: result = userGoal.includes('!'); //re-run this code whenever any of the referenced values change
    
</script>

<main>
	<h3 class="{result ? 'isWrong' : ''}"> {userGoal} </h3>
</main>

<style>
	.isWrong{
		color:red;
	}
</style>