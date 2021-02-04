<script>
  export let cityImg = 'images/london.png';
  const componentFunctions = () => {
    console.log('component log');
  };
</script>

<div class="right-panel panel">
  <img src={cityImg} alt="" width="120" on:click={componentFunctions} />
</div>
