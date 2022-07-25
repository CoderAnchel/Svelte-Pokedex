<script>
    export  let pokeman;
</script>
<a class="xdi" href={`/pokemon/${pokeman.id}`} >
    <img class="h-40 w-40 " src={pokeman.image} alt={pokeman.name}/>
    <h2 class="lmo">{pokeman.id}. {pokeman.name}</h2>
</a>

<style>
    .xdi {
        background: #f6f8fc;
        width: 40%;
        text-decoration: none !important;
        margin: 10px;
        border-radius: 10px;
    }

    .lmo {
        color: black;
    }

</style>