<script>
  export let food;
</script>

<div class="card">
  <a href="/src/components/food-detail.svelte"><img src={food.image} alt={food.title} /></a>
  <h3>{food.title}</h3>
</div>

<style>
  .card{
    margin: 20px;
    padding: 5px;
    
  }
  img{
    width:100%;
    border-radius: 5px;
  }
  h3{
    font-size: 1.5rem;
    text-align: center;
  }
</style>