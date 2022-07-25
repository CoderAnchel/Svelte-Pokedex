<script>
    import image from "../assets/Pokemon-Logo.png"
    import logo from "../assets/logo.png"
    import pika from "../assets/pika.png"

</script>

<svelte:head>
    <title>PokeSvelte Kit</title>
</svelte:head>

<div class="container">
    <h1 class="title">SvelteKit <img src={logo} alt=""> </h1>
    <div class="wrapper">
        <p class="desc">What are you looking for?</p>
        <a href="/pokemon" class="poke">
            <span>Pokémon</span>
        </a>
        <div class="secon">   
            <a href="/pokemon" class="poke2">
                <span>Items</span>
            </a>
            <a href="/pokemon" class="poke3">
                <span>types</span>
            </a>
        </div>
    </div>
</div>

<div class="card">
    <img src={pika} alt="">
    <span class="some">Maded By Anchel </span>
    <a href="github.com">Code</a>
</div>

<style>

    
    .container {
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
        position: relative;
        top: -40px;
    }

    .title {
        font-size: 45px;
        display: flex;
        align-items: center;
        text-transform: uppercase;
    }

    .title img {
        width: 300px;;
        position: relative;
        top: -10px;
    }

    .desc  {
        font-size: 20px;
        margin-bottom: 10px;
    }

    .wrapper {
        width: 100%;
        max-width: 700px;
        position: relative;
        top: -60px;
    }

    .poke {
        background: #f7776a;
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 20px;
        margin-top: 20px;
        transition: all 0.3s;
        text-decoration: none;
        color: #ffff;
    }

    .poke span {
        font-size: 40px;
        font-weight: 600;
    }

    .poke:hover {
        height: 120px;
    }

    .poke2 {
        background: #58a9f4;
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 20px;
        margin-top: 20px;
        transition: all 0.3s;
        text-decoration: none;
        color: #ffff;
    }

    .poke2 span {
        font-size: 40px;
        font-weight: 600;
    }

    .poke3 {
        background: #ffce4b;
        height: 100px;
        display: flex;
        align-items: center;
        justify-content: center;
        border-radius: 20px;
        margin-top: 20px;
        transition: all 0.3s;
        text-decoration: none;
        color: #ffff;
    }

    .poke3 span {
        font-size: 40px;
        font-weight: 600;
    }

    .poke2:hover {
        height: 120px;
        cursor: pointer;
    }

    .poke3:hover {
        height: 120px;
        cursor: pointer;
    }

    .card {
        position: absolute !important;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        bottom: 50px;
        right: 20px;
        border-radius: 10px;
        background: #f6f8fc;
        width: 300px;
        color: #0000;
        height: 100px;
    }

    .some {
        color: #000 !important;
        font-size: 20px;
        font-weight: 600;
    }

    .card img {
        position: absolute;
        width: 70px;
        top: -40px;
        left: -24px;
    }

    .card a {
        font-size: 20px;
        text-decoration: none;
        color: #58a9f4;
        text-transform: uppercase;
        font-weight: 600;
        font-family: 600;
        margin-top: 10px;
    }
</style>