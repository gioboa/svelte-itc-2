<script>
  import { createEventDispatcher } from 'svelte';

  export let date;
  export let city = 'Paris';
  export let img = 'images/cloudy.png';
  export let deg = '15';

  const dispatch = createEventDispatcher();

  const onClick = () => {
    dispatch('message', { data: 'click from child!' });
  };
</script>

<div class="left-panel panel">
  <div class="date">{date}</div>
  <div class="city">{city}</div>
  <div class="temp">
    <img src={img} alt="" width="60" on:click={onClick} />
    {deg}&deg;
  </div>
</div>
