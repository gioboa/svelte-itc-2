<script>
  import './App.css';

  export let title;
</script>

<main>
  <div class="widget">
    <div class="left-panel panel">
      <div class="date">Monday, 20 Aug 2018</div>
      <div class="city">
        {title}
      </div>
      <div class="temp">
        <!-- <img src="https://s5.postimg.cc/yzcm7htyb/image.png" alt="" width="60" /> -->
        18&deg;
      </div>
    </div>
    <div class="right-panel panel">
      <img src="images/london.png" alt="" width="120" />
    </div>
  </div>
</main>
