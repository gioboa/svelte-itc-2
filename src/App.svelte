<script>
  import './App.css';
  import LeftPanel from './components/LeftPanel.svelte';
  import RightPanel from './components/RightPanel.svelte';

  let currentDate = new Date().toLocaleTimeString();
  let city = 'London';
  let data = {
    img: 'images/sun.png',
    deg: '22',
  };
  let cityImg = 'images/parigi.png';

  const parentFunctions = (event) => {
    console.log(`parent log - ${event.detail.data}`);
  };
</script>

<main>
  <div class="widget">
    <LeftPanel date={currentDate} {city} on:message={parentFunctions} />
    <RightPanel />
  </div>
  <div class="widget">
    <LeftPanel date={currentDate} {...data} />
    <RightPanel {cityImg} />
  </div>
</main>
