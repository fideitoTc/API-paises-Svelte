<script>
    //importamos el componente parImpar:svelte y lo llamamos parImpar
  import ParImpar from './lib/parImpar.svelte';
  let valor=0;
    //escuchamos el evento imput
  const listenInput = (event) => valor = event.target.value
</script>

<main>
  <!--llamamos el componente ingresando un numero impar en este caso 5-->
    <ParImpar numero={valor}/>
  <!--llamamos nuevamente el componente ingresando un numero par en este caso 20-->

  <input value={valor} on:input={listenInput}>
</main>