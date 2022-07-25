<script>
    import pokedex from "../assets/pokedex.png";
    import logo from "../assets/logo.png"

    import { pokemon } from "../stores/pokestores";
import Pokemancard from "../components/pokemancard.svelte";

    console.log($pokemon)
</script>

<span class="xdi"><a href="/">Home</a></span>

<div class="container">
    <div class="row">
        <img class="xd" src={pokedex} alt="">
        <img class="logo" src={logo} alt="">
    </div>

    <div class="rowww">
        {#each $pokemon as pokeman}
            <Pokemancard pokeman={pokeman}/>
        {/each}
    </div>
</div>

<style>

    .rowww {
        width: 100%;
        max-width: 800px;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
    }

    .row {
        display: flex;
        align-items: center;
    }

    .xd {
        width: 80px;
    }

    .logo {
        width: 180px !important;
    }

    .xdi {
        background: #ffff;
        padding: 10px;
        position: relative;
        top: 10px;
        border-radius: 5px;
    }

    .xdi a {
        color: #000 !important;
        text-decoration: none;
    }
</style>