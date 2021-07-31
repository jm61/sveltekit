<script>
const c = console.log
import {pokemon}  from '../stores/pokestore'
import PokemanCard from '../components/pokemanCard.svelte';
</script>

<svelte:head>
    <title>Home Svelte Pokedex</title>
</svelte:head>

<h1 class="text-2xl text-center my-8 uppercase">Svelte Kit Pokedex</h1>

<div class="py-4 grid gap-4 md:grid-cols-2 grid-cols-1">
    {#each $pokemon as pokeman }
   <PokemanCard {pokeman}></PokemanCard>
{/each}
</div>
