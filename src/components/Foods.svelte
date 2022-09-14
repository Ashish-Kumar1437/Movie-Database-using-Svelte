<script>
  export let foods;
  import FoodCard from "./Food-card.svelte";
</script>

<div class="container">
  {#each foods as food}
    <FoodCard {food} />
  {/each}
</div>

<style>
  .container{
    display: grid;
    grid-template-columns: repeat( auto-fit, minmax(300px, 1fr) );
    
  }
</style>
