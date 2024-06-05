<script>
    export let numero; //exportamos la variable numero para poder llamarlo en app.svelte
    let resultado;   //variable local
    $: if (numero===0)
        resultado="neutro";
    else
        if (numero%2===0)
            resultado="par";
        else
            resultado="impar";
</script>
<!---las variables las llamamos entre llaves-->
<p>el numero {numero} es {resultado} </p>
<style>
    p{
        color: black;
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        font-size: 25px;
    }
</style>