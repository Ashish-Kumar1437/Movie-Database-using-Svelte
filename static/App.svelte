<script>
  import { onMount } from "svelte";
  import FoodCardSection from "./components/Foods.svelte";
  import Movie from "./components/Foods.svelte";
  let foods = [];

  onMount(async () => {
    const url = `https://api.spoonacular.com/recipes/complexSearch?apiKey=6dbebac7ae3a44b695bd25d31075cb84`;
    const res = await fetch(url);
    const { results } = await res.json();
    foods = results;
  });
</script>

<FoodCardSection {foods} />
